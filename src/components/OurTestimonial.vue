<script setup>
import rasaline1 from "../assets/images/rasaline1.png";
import rasaline2 from "../assets/images/rasaline2.png";
import rasaline3 from "../assets/images/rasaline3.png";
import goldrightarrow from "../assets/icons/gold-arrow-right.svg";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <p class="testimonial">Testimonial</p>
                <h2>Our latest news</h2>
                <div class="cards">
                    <div class="card">
                        <img :src="rasaline1" alt="" />
                        <div class="content">
                            <div class="top">
                                <h4><span>By:</span> rasaline</h4>
                                <p>23.01.2021</p>
                            </div>
                            <h3>Ideal cocktails from barmen....</h3>
                            <button>
                                Read More
                                <img
                                    class="arrow"
                                    :src="goldrightarrow"
                                    alt=""
                                />
                            </button>
                        </div>
                    </div>
                    <div class="card">
                        <img :src="rasaline2" alt="" />
                        <div class="content">
                            <div class="top">
                                <h4><span>By:</span> rasaline</h4>
                                <p>23.01.2021</p>
                            </div>
                            <h3>Ideal cocktails from barmen....</h3>
                            <button>
                                Read More
                                <img
                                    class="arrow"
                                    :src="goldrightarrow"
                                    alt=""
                                />
                            </button>
                        </div>
                    </div>
                    <div class="card">
                        <img :src="rasaline3" alt="" />
                        <div class="content">
                            <div class="top">
                                <h4><span>By:</span> rasaline</h4>
                                <p>23.01.2021</p>
                            </div>
                            <h3>Ideal cocktails from barmen....</h3>
                            <button>
                                Read More
                                <img
                                    class="arrow"
                                    :src="goldrightarrow"
                                    alt=""
                                />
                            </button>
                        </div>
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
    gap: 20px;
    justify-content: space-between;
}
.card {
    width: 366px;
    height: 528px;
    background-color: #1c1814;
}
.content {
    padding: 20px 24px 24px;
}
.top {
    display: flex;
    align-items: center;
    justify-content: space-between;
}
.top h4 {
    font-size: 18px;
    color: #ffffff;
}
.top h4 span {
    color: #c99e71;
}
.top p {
    font-size: 18px;
    color: #ffffff;
}
h3 {
    margin: 16px 0 32px 0;
    font-family: R-Regular;
    color: #ffffff;
    text-align: start;
    font-size: 20px;
}
button {
    font-family: U-Medium;
    font-size: 16px;
    color: #c99e71;
    display: flex;
    gap: 8px;
    align-items: center;
    background-color: transparent;
}
@media only screen and (max-width: 1200px) {
    .testimonial {
        font-size: 17px;
    }
    h2 {
        font-size: 40px;
    }
    .cards {
        display: flex;
        gap: 40px 25px;
        flex-wrap: wrap;
        justify-content: space-evenly;
    }
}
@media only screen and (max-width: 815px) {
    .testimonial {
        font-size: 16px;
    }
    h2 {
        font-size: 36px;
    }

    .card {
        display: flex;
        width: 100%;
        height: auto;
        align-items: center;
        justify-content: space-evenly;
        padding: 0 20px;
    }
    .card img {
        width: 40%;
    }
    button {
        font-size: 13px;
        width: 130px;
    }
    .arrow {
        max-width: 25px;
    }
}
@media only screen and (max-width: 565px) {
    .testimonial {
        font-size: 16px;
    }
    h2 {
        font-size: 28px;
    }

    .card {
        display: flex;
        flex-direction: column;
        padding: 20px 0;
        gap: 20px;
        width: 100%;
        height: auto;
        align-items: center;
        justify-content: space-evenly;
    }
    .card img {
        width: 30%;
    }
    h3 {
        font-size: 17px;
    }
    .arrow {
        max-width: 25px;
    }
}
</style>
