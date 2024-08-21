<script setup>
import coffemachine from "../assets/images/coffemachine.png";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <img :src="coffemachine" alt="" />
                <div class="content">
                    <h2>
                        Coffee <br />
                        machine, buy for home
                    </h2>
                    <p>
                        mauris rhoncus in imperdiet placerat. vestibu emismd
                        nisl suscirpit ligula volutpat, a feyguat urn maxmaus.
                        cars massa nibhtincidunt. donec et nib maximus, est eu,
                        mattis nuce.
                        <span
                            >preasent ut quam quis quam venen atis fri ngilla.
                            morbi vastibulum id tells mmodo mattis. aliauam erat
                            volutpal.</span
                        >
                    </p>
                    <button>Discover now</button>
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
    background-color: #1c1814;
    display: flex;
    justify-content: space-between;
    padding: 72px 89px 84px;
}
img {
    margin: 13px 0 0 80px;
}
.content {
    display: flex;
    flex-direction: column;
    gap: 36px;
    max-width: 526px;
    width: 100%;
}
h2 {
    font-family: R-Regular;
    font-size: 48px;
    line-height: 130%;
    color: #ffffff;
}
p {
    font-family: U-Medium;
    font-size: 16px;
    color: rgba(255, 255, 255, 0.8);
    line-height: 180%;
    text-transform: capitalize;
}
button {
    width: 215px;
    height: 62px;
    color: #fff;
    background-color: #c99e71;
    text-transform: uppercase;
    font-family: I-Bold;
}
@media only screen and (max-width: 1100px) {
    .wrapper {
        padding: 52px 69px 64px;
    }
}
@media only screen and (max-width: 1050px) {
    .content {
        max-width: 526px;
    }
    h2 {
        font-size: 40px;
    }
    p {
        font-size: 15px;
    }
    button {
        width: 215px;
        height: 62px;
    }
    img {
        margin: 13px 0 0 60px;
    }
}
@media only screen and (max-width: 1025px) {
    .content {
        max-width: 476px;
    }
    h2 {
        font-size: 36px;
    }
    p {
        font-size: 15px;
    }
    button {
        width: 205px;
        height: 52px;
    }
    img {
        margin: 13px 0 0 40px;
    }
}
@media only screen and (max-width: 965px) {
    .content {
        max-width: 436px;
        justify-content: center;
    }
    h2 {
        font-size: 32px;
    }
    p {
        font-size: 14px;
    }
    button {
        width: 205px;
        height: 52px;
    }
    img {
        width: 30%;
        margin: 0;
    }
}
@media only screen and (max-width: 860px) {
    .content {
        max-width: 396px;
        gap: 25px;
    }
    h2 {
        font-size: 30px;
    }
    p {
        font-size: 14px;
    }
    button {
        width: 190px;
        height: 42px;
    }
    img {
        width: 30%;
        margin: 0;
    }
}
@media only screen and (max-width: 795px) {
    .content {
        max-width: 396px;
        gap: 25px;
    }
    h2 {
        font-size: 28px;
    }
    p {
        font-size: 14px;
    }
    button {
        width: 190px;
        height: 42px;
        font-size: 15px;
    }
    img {
        width: 30%;
        margin: 0;
    }
    .wrapper {
        padding: 50px;
    }
}
@media only screen and (max-width: 760px) {
    .content {
        max-width: 100%;
        gap: 25px;
        align-items: center;
    }

    button {
        width: 190px;
        height: 42px;
        font-size: 15px;
    }

    .wrapper {
        flex-direction: column;
        padding: 50px;
        text-align: center;
        align-items: center;
        gap: 30px;
    }
}
@media only screen and (max-width: 450px) {
    h2 {
        font-size: 24px;
    }
    p {
        font-size: 13px;
    }
    p span {
        display: none;
    }
    button {
        width: 160px;
        height: 32px;
        font-size: 14px;
    }
}
</style>
