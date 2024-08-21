<script setup>
import coffebag from "../assets/images/coffebag.png";
import goldstar from "../assets/icons/goldstar.svg";
import star from "../assets/icons/star.svg";
import shoppingbag from "../assets/icons/shopping-bag.svg";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <p class="pp">Popular Product</p>
                <h2>Coffee popular Product</h2>
                <div class="cards">
                    <div class="card">
                        <img :src="coffebag" alt="" />
                        <h3 class="h3">brazil coffee gred</h3>
                        <button>
                            <img :src="shoppingbag" alt="" />Add to cart
                        </button>
                    </div>
                    <div class="card">
                        <img class="coffebag" :src="coffebag" alt="" />
                        <div>
                            <div class="rate">
                                <p>coffee</p>
                                <div class="stars">
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="star" alt="" /></span>
                                </div>
                            </div>
                            <h3>brazil coffee gred</h3>
                            <p class="price">
                                Price - <span class="span1"> $320.00/ </span>
                                <span class="span2">$358</span>
                            </p>
                        </div>
                    </div>
                    <div class="card">
                        <img class="coffebag" :src="coffebag" alt="" />
                        <div>
                            <div class="rate">
                                <p>coffee</p>
                                <div class="stars">
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="goldstar" alt="" /></span>
                                    <span><img :src="star" alt="" /></span>
                                </div>
                            </div>
                            <h3>brazil coffee gred</h3>
                            <p class="price">
                                Price - <span class="span1"> $320.00/ </span>
                                <span class="span2">$358</span>
                            </p>
                        </div>
                    </div>
                </div>
                <button class="view">View all product</button>
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
    flex-direction: column;
    align-items: center;
}
.pp {
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
    width: 100%;
    display: flex;
    justify-content: space-between;
}
.card {
    padding: 48px;
    width: 366px;
    height: 579px;
    background-color: #121315;
    text-align: center;
}
.rate {
    display: flex;
    gap: 13px;
    align-items: center;
    justify-content: center;
    margin-top: 36px;
    margin-bottom: 20px;
}
.rate p {
    color: #c99e71;
    text-transform: uppercase;
}
.rate span {
    display: grid;
    place-content: center;
    width: 20px;
    height: 20px;
}
.stars {
    display: flex;
    align-items: center;
    gap: 4px;
}
h3 {
    font-family: R-Regular;
    font-size: 24px;
    color: #ffffff;
    text-transform: uppercase;
}
.price {
    color: #ffffff;
    text-transform: uppercase;
    font-family: U-Semibold;
    margin-top: 20px;
}
.price .span1 {
    color: #c99e71;
}
.price .span2 {
    text-decoration: line-through;
}
.card button {
    width: 169px;
    height: 48px;
    display: flex;
    align-items: center;
    gap: 12px;
    background-color: #c99e71;
    color: white;
    justify-content: center;
    font-family: U-Semibold;
    font-size: 18px;
    margin: 0 auto;
}
.card button img {
    width: 24px;
    height: 24px;
}
.h3 {
    margin: 36px 0;
}
.view {
    margin-top: 56px;
    width: 252px;
    height: 62px;
    background-color: #c99e71;
    font-family: I-Bold;
    color: #ffffff;
    font-size: 18px;
    text-transform: uppercase;
}
@media only screen and (max-width: 1190px) {
    .card {
        padding: 32px;
        width: 336px;
        height: 549px;
        background-color: #121315;
        text-align: center;
    }
}
@media only screen and (max-width: 1100px) {
    .card {
        padding: 24px;
        width: 326px;
        height: 519px;
    }
    .rate {
        margin-top: 24px;
        margin-bottom: 20px;
    }
    .h3 {
        margin: 24px 0;
    }
}
@media only screen and (max-width: 1060px) {
    .card:first-child {
        display: none;
    }
    .card {
        padding: 24px;
        width: 460px;
    }
}
@media only screen and (max-width: 995px) {
    .card {
        padding: 24px;
        width: 430px;
    }
}
@media only screen and (max-width: 935px) {
    .card {
        padding: 24px;
        width: 410px;
    }
}
@media only screen and (max-width: 890px) {
    .card {
        padding: 24px;
        width: 380px;
    }
    .view {
        width: 232px;
        height: 52px;
    }
}
@media only screen and (max-width: 830px) {
    .card {
        padding: 24px;
        width: 350px;
        height: 519px;
    }
    .view {
        width: 222px;
        height: 47px;
        font-size: 16px;
    }
}
@media only screen and (max-width: 770px) {
    .card {
        padding: 24px;
        width: 100%;
        height: auto;
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
    }
    .coffebag {
        width: 30%;
    }
    .cards {
        width: 100%;
        display: flex;
        justify-content: space-between;
        flex-direction: column;
        row-gap: 20px;
    }
    .view {
        width: 202px;
        height: 47px;
        font-size: 15px;
    }
}
@media only screen and (max-width: 600px) {
    .pp {
        font-size: 16px;
    }
    h2 {
        font-size: 35px;
    }
    h3 {
        font-size: 21px;
    }
}
@media only screen and (max-width: 480px) {
    .pp {
        font-size: 15px;
    }
    h2 {
        font-size: 32px;
        margin: 12px 0 48px;
    }
    h3 {
        font-size: 19px;
    }
}
@media only screen and (max-width: 450px) {
    .card {
        padding: 24px;
        width: 100%;
        height: auto;
        display: flex;
        flex-direction: column;
        justify-content: space-evenly;
        align-items: center;
    }

    h2 {
        text-align: center;
    }
    h3 {
        font-size: 17px;
    }
    .view {
        width: 192px;
        height: 42px;
        font-size: 14px;
    }
}
</style>
