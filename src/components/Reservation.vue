<script setup></script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <div class="map"></div>
                <form action="" class="form">
                    <p class="reservation">Reservation</p>
                    <h2>Booking a table</h2>
                    <div class="inputs">
                        <input type="text" placeholder="4 person" />
                        <input type="text" placeholder="12.25, 2020" />
                        <input type="text" placeholder="11:00 AM" />
                    </div>
                    <button>BOOK S TABLE</button>
                </form>
            </div>
        </div>
    </section>
</template>

<style scoped>
h1,
h2,
h3,
h4,
h5,
h6,
p {
    margin: 0;
    padding: 0;
}

.wrapper {
    display: flex;
}
.reservation {
    color: #c99e71;
    font-family: U-Semibold;
    font-size: 18px;
}
h2 {
    font-family: R-Regular;
    font-size: 48px;
    color: #ffffff;
    margin: 12px 0 58px;
}
.form {
    max-width: 585px;
    width: 100%;
    padding: 72px 48px;
    background-color: #1c1814;
    text-align: center;
}
.inputs {
    display: flex;
    flex-direction: column;
    gap: 24px;
}
.map {
    background-image: url(../assets/images/map.png);
    background-repeat: no-repeat;
    max-width: 585px;
    width: 100%;
    background-position: center center;
    background-size: cover;
}
input {
    height: 64px;
    width: 100%;
    background-color: #14110e;
    padding: 0 20px;
    font-size: 18px;
    color: #ffffff;
}
input::placeholder {
    color: #ffffffca;
}
button {
    margin-top: 56px;
    background-color: #c99e71;
    width: 202px;
    height: 62px;
    font-family: I-Bold;
    font-size: 18px;
    color: white;
}
@media only screen and (max-width: 1091px) {
    .reservation {
        font-size: 17px;
    }
    h2 {
        font-size: 40px;
    }
    .map {
        max-width: 585px;
        width: 100%;
    }
}
@media only screen and (max-width: 785px) {
    .reservation {
        font-size: 15px;
    }
    h2 {
        font-size: 32px;
    }
    button {
        width: 180px;
        height: 32px;
        font-size: 15px;
    }
}
@media only screen and (max-width: 680px) {
    .reservation {
        font-size: 15px;
    }
    h2 {
        font-size: 28px;
    }
    .map {
        height: 200px;
        max-width: 728px;
        width: 100%;
    }

    .form {
        max-width: 100%;
    }
    .wrapper {
        flex-direction: column;
    }
    .form {
        width: 100%;
        padding: 52px 28px;
        background-color: #1c1814;
        text-align: center;
    }
    button {
        width: 160px;
        height: 32px;
        font-size: 15px;
    }
}
</style>
