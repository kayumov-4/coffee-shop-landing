<script setup>
import johnsmith from "../assets/images/johnsmith.jpg";
import bretlee from "../assets/images/bretlee.jpg";
import goldstar from "../assets/icons/goldstar2.svg";
import arrowright from "../assets/icons/arrow-right.svg";
import arrowleft from "../assets/icons/arrow-left.svg";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <p class="testimonial">Testimonial</p>
                <h2>Says our customers</h2>
                <div class="cards">
                    <div class="card">
                        <div class="top">
                            <img :src="johnsmith" alt="" />
                            <p>
                                Education WP is a special build for effective
                                education & Learning Management System site.
                                <span
                                    >Education WP is the next generation & one
                                    of the best education WordPress themes which
                                    all the strength of eLearning WP..</span
                                >
                            </p>
                        </div>
                        <div class="bottom">
                            <div class="content">
                                <h3>John Smith</h3>
                                <p>Product Designer</p>
                            </div>
                            <div class="stars">
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                            </div>
                        </div>
                    </div>
                    <div class="card">
                        <div class="top">
                            <img :src="bretlee" alt="" />
                            <p>
                                Education WP is a special build for effective
                                education & Learning Management System site.
                                <span
                                    >Education WP is the next generation & one
                                    of the best education WordPress themes which
                                    all the strength of eLearning WP..</span
                                >
                            </p>
                        </div>
                        <div class="bottom">
                            <div class="content">
                                <h3>Brett Lee</h3>
                                <p>User Experience Designer</p>
                            </div>
                            <div class="stars">
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                                <img :src="goldstar" alt="" />
                            </div>
                        </div>
                    </div>
                </div>
                <div class="next">
                    <div class="sts">
                        <p>2/6 People</p>
                        <div class="of">
                            <span></span>
                        </div>
                    </div>
                    <div class="arrows">
                        <button><img :src="arrowleft" alt="" /></button>
                        <button><img :src="arrowright" alt="" /></button>
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
.testimonial {
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
    display: flex;
    justify-content: space-between;
    gap: 20px;
}
.card {
    max-width: 565px;
    width: 100%;
    background-color: #1c1814;
    padding: 40px 40px 37px;
}
.top {
    display: flex;
    gap: 24px;
    margin-bottom: 28px;
}
.top p {
    text-align: left;
}
p {
    color: rgba(255, 255, 255, 0.8);
    line-height: 180%;
    text-transform: capitalize;
}
.bottom {
    display: flex;
    justify-content: space-between;
    align-items: end;
    text-align: left;
}
.bottom h3 {
    color: #ffffff;
    font-size: 18px;
    line-height: 120%;
    margin-bottom: 4px;
}
.bottom p {
    font-size: 14px;
    color: rgba(255, 255, 255, 0.5);
}
.stars {
    display: flex;
    gap: 4px;
}
.next {
    display: flex;
    align-items: center;
    justify-content: space-between;
    margin-top: 36px;
}
.sts {
    display: flex;
    flex-direction: column;
    gap: 20px;
    text-align: start;
}
.sts p {
    font-family: U-Semibold;
    font-size: 20px;
    color: #c99e71;
}
.of {
    width: 120px;
    height: 4px;
    background-color: #1c1814;
    border-radius: 3px;
}
.of span {
    width: 50px;
    display: block;
    background-color: #c99e71;
    height: 4px;
}
.arrows {
    display: flex;
    gap: 16px;
}
.arrows button {
    width: 56px;
    height: 56px;
    display: grid;
    place-content: center;
    border-radius: 100%;
}
.arrows button:first-child {
    background-color: #121315;
}
.arrows button:last-child {
    background-color: #c99e71;
}
@media only screen and (max-width: 1200px) {
    .cards {
        gap: 40px;
    }
    .top {
        flex-direction: column;
    }
}
@media only screen and (max-width: 812px) {
    .testimonial {
        font-size: 16px;
    }
    h2 {
        font-size: 40px;
    }
    .cards {
        gap: 20px;
    }
    .top p {
        text-align: center;
        font-size: 15px;
    }
    .top p span {
        display: none;
    }
    .bottom {
        flex-direction: column;
        align-items: center;
        text-align: center;
        gap: 20px;
    }
}
@media only screen and (max-width: 588px) {
    .testimonial {
        font-size: 15px;
    }
    h2 {
        font-size: 36px;
    }
    .cards {
        flex-direction: column;
    }
    .bottom h3 {
        font-size: 16px;
    }
}
</style>
