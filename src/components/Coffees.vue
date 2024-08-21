<script setup>
import bestcoffe from "../assets/images/bestcoffe.png";
import placetogetlost from "../assets/images/placetogetlost.png";
import roesting from "../assets/images/roesting.png";
import rightarrow from "../assets/icons/arrow-right.svg";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <div class="card">
                    <h4><span>01</span>Best Coffee Flavour</h4>
                    <img :src="bestcoffe" alt="" />
                </div>
                <div class="card">
                    <h4><span>02</span>Place to get lost</h4>
                    <img :src="placetogetlost" alt="" />
                </div>
                <div class="card">
                    <h4><span>03</span>Proper roesting</h4>
                    <img :src="roesting" alt="" />
                </div>
                <button><img :src="rightarrow" alt="" /></button>
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
    justify-content: space-between;
    align-items: center;
}
.card {
    display: flex;
    flex-direction: column;
    gap: 24px;
    width: 360px;
    height: 474px;
}
h4 {
    font-family: R-Regular;
    font-size: 24px;
    color: white;
}
h4 span {
    color: #c99e71;
    margin-right: 12px;
}
button {
    font-family: U-Medium;
    font-size: 16px;
    background-color: #c99e71;
    border-radius: 100%;
    display: none;
    padding: 10px;
    align-items: center;
}
@media only screen and (max-width: 1170px) {
    .card {
        width: 330px;
        height: 444px;
    }
}
@media only screen and (max-width: 1080px) {
    .card {
        width: 300px;
        height: 404px;
    }
}
@media only screen and (max-width: 1080px) {
    .card {
        width: 280px;
        height: 380px;
    }
    h4 {
        font-size: 20px;
    }
}
@media only screen and (max-width: 930px) {
    .card {
        width: 260px;
        height: 360px;
    }
    h4 {
        font-size: 18px;
    }
}
@media only screen and (max-width: 870px) {
    .card {
        width: 360px;
        height: 474px;
    }
    .card:nth-child(3) {
        display: none;
    }
    h4 {
        font-size: 18px;
    }
    button {
        display: flex;
    }
}
@media only screen and (max-width: 840px) {
    .card {
        width: 310px;
        height: 414px;
    }
    .card:nth-child(3) {
        display: none;
    }
    h4 {
        font-size: 18px;
    }
}
@media only screen and (max-width: 755px) {
    .card {
        width: 280px;
        height: 390px;
    }
    .card:nth-child(3) {
        display: none;
    }
    h4 {
        font-size: 16px;
    }
}
@media only screen and (max-width: 690px) {
    .card {
        width: 250px;
        height: 360px;
    }

    h4 {
        font-size: 17px;
    }
}
@media only screen and (max-width: 620px) {
    .card {
        width: 220px;
        height: 330px;
    }
    h4 {
        font-size: 16px;
    }
}
@media only screen and (max-width: 575px) {
    .card {
        width: 180px;
        height: 290px;
    }
    h4 {
        font-size: 15px;
    }
    button {
        padding: 5px;
    }
}
@media only screen and (max-width: 490px) {
    .card {
        width: 340px;
        height: 444px;
    }
    .card:nth-child(2) {
        display: none;
    }
    h4 {
        font-size: 19px;
    }
}
@media only screen and (max-width: 490px) {
    .card {
        width: 300px;
        height: 404px;
    }

    h4 {
        font-size: 17px;
    }
}
@media only screen and (max-width: 420px) {
    .card {
        width: 230px;
        height: 350px;
    }

    h4 {
        font-size: 16px;
    }
}
</style>
