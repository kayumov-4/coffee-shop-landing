<script setup>
import americano1 from "../assets/images/americano1.png";
import americano2 from "../assets/images/americano2.png";
import americano3 from "../assets/images/americano3.png";
import americano4 from "../assets/images/americano4.png";
import americano5 from "../assets/images/americano5.png";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <p class="menu">Menu</p>
                <h2>Coffee popular menu</h2>
                <div class="cards">
                    <div class="card">
                        <div class="content">
                            <img :src="americano1" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano2" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano3" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano4" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano5" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano1" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano3" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                    <div class="card">
                        <div class="content">
                            <img :src="americano3" alt="" />
                            <h4>Americano rosted gred</h4>
                        </div>
                        <p>$12:00</p>
                    </div>
                </div>
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
    text-align: center;
}
.menu {
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
.cards {
    display: grid;
    grid-template-columns: auto auto;
    row-gap: 36px;
    column-gap: 40px;
}
.card {
    max-width: 565px;
    width: 100%;
    padding: 24px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border: 1px solid #32323d;
}
.content {
    display: flex;
    align-items: center;
    gap: 20px;
}
.card h4 {
    font-family: R-Regular;
    color: #ffffff;
    font-size: 24px;
}
.card p {
    color: #c99e71;
    font-size: 18px;
    font-family: U-Semibold;
}
@media only screen and (max-width: 1010px) {
    .card h4 {
        font-size: 20px;
    }
    .card p {
        font-size: 17px;
    }
    .cards {
        gap: 30px;
    }
}
@media only screen and (max-width: 915px) {
    .card h4 {
        font-size: 18px;
    }
    .card p {
        font-size: 16px;
    }
    .cards {
        gap: 20px;
    }
}
@media only screen and (max-width: 850px) {
    .card:nth-child(5) {
        display: none;
    }
    .card:nth-child(6) {
        display: none;
    }
    .card:nth-child(7) {
        display: none;
    }
    .card:nth-child(8) {
        display: none;
    }
    .card {
        gap: 20px;
    }
    .menu {
        font-size: 17px;
    }
    h2 {
        font-size: 40px;
    }
}
@media only screen and (max-width: 695px) {
    .cards {
        width: 100%;
        grid-template-columns: auto;
    }
    .card {
        max-width: 638px;
        width: 100%;
        padding: 20px;
    }

    .card:nth-child(4) {
        display: none;
    }
    .menu {
        font-size: 15px;
    }
    h2 {
        font-size: 35px;
    }
}
</style>
