<script setup>
import placetogetlost from "../assets/images/placetogetlost.png";
import bestcoffe from "../assets/images/bestcoffe.png";
import createnewstory from "../assets/images/createnewstory.png";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <div class="grid">
                    <div class="a"></div>
                    <div class="b"></div>
                    <div class="c"></div>
                </div>
                <div class="history">
                    <h4>Our history</h4>
                    <h5>Create a new story with us</h5>
                    <p>
                        mauris rhoncus in imperdiet placerat. vestibu emismd
                        nisl suscirpit ligula volutpat, a feyguat urn maxmaus.
                        cars massa nibhtincidunt. donec et nibh maximus, est eu,
                        mattis nuce. preasent ut quam quis quam venen atis
                        fringilla. morbi vastibulum id tells mmodo mattis.
                        aliauam erat volutpal.
                    </p>
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
    display: flex;
    gap: 32px;
}
.grid {
    display: grid;
    grid-template-columns: auto auto;
    gap: 32px;
    grid-template-areas:
        "a c"
        "b c";
    width: 628px;
}
.a {
    grid-area: a;
    background-image: url(../assets/images/placetogetlost.png);
    background-repeat: no-repeat;
    background-position: top;
}
.b {
    grid-area: b;
    background-image: url(../assets/images/bestcoffe.png);
    background-repeat: no-repeat;
    background-position: bottom;
}
.c {
    grid-area: c;
    background-image: url(../assets/images/createnewstory.png);
    background-repeat: no-repeat;
    background-position: top;
}
.history {
    padding: 120px 56px;
    background-color: #1c1814;
    height: 635px;
    width: 510px;
}
h4 {
    font-family: U-Semibold;
    font-size: 18px;
    color: #c99e71;
}
h5 {
    font-family: R-Regular;
    font-size: 48px;
    line-height: 130%;
    color: #fff;
    margin: 12px 0 36px;
}
p {
    font-family: U-Medium;
    color: rgba(255, 255, 255, 0.8);
    line-height: 180%;
    text-transform: capitalize;
}
@media only screen and (max-width: 965px) {
    .wrapper {
        gap: 20px;
    }
    .grid {
        gap: 20px;
    }
    .history {
        padding: 100px 56px;
        height: 605px;
        width: 490px;
    }
    h4 {
        font-size: 16px;
    }
    h5 {
        font-size: 40px;
    }
    p {
        font-size: 15px;
    }
}
@media only screen and (max-width: 850px) {
    .wrapper {
        gap: 20px;
    }
    .grid {
        gap: 20px;
    }
    .history {
        padding: 80x 46px;
        height: 605px;
        width: 490px;
    }
    h4 {
        font-size: 16px;
    }
    h5 {
        font-size: 36px;
    }
    p {
        font-size: 14px;
    }
}
@media only screen and (max-width: 780px) {
    .wrapper {
        flex-direction: column;
        gap: 20px;
    }
    .grid {
        width: 100%;
        gap: 20px;
        height: 550px;
    }
    .history {
        padding: 80x 46px;
        height: 405px;
        width: 100%;
    }
    h4 {
        font-size: 16px;
    }
    h5 {
        font-size: 36px;
    }
    p {
        font-size: 14px;
    }
}
@media only screen and (max-width: 625px) {
    .wrapper {
        gap: 20px;
    }
    .grid {
        width: 100%;
        gap: 20px;
        height: 550px;
    }
    .history {
        padding: 60px 36px;
        height: 405px;
        width: 100%;
    }
    h4 {
        font-size: 15px;
    }
    h5 {
        font-size: 32px;
    }
    p {
        font-size: 14px;
    }
}
@media only screen and (max-width: 535px) {
    .grid {
        height: 450px;
    }
    .history {
        padding: 60px 30px;
        height: auto;
        width: 100%;
    }
    h4 {
        font-size: 15px;
    }
    h5 {
        font-size: 28px;
    }
    p {
        font-size: 14px;
    }
}
@media only screen and (max-width: 420px) {
    .grid {
        height: 380px;
    }
    .history {
        padding: 60px 30px;
        height: auto;
        width: 100%;
    }
    h4 {
        font-size: 15px;
    }
    h5 {
        font-size: 28px;
    }
    p {
        font-size: 14px;
    }
}
</style>
