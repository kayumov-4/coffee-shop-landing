<script setup>
import playbtn from "../assets/icons/playvideo.svg";
</script>
<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <div class="content">
                    <h1>Enjoy Your Morning Coffee.</h1>
                    <p>
                        The coofee is brewed by fist roasting the green coffee
                        beans over hot coals in brazier. given to Opportunity
                    </p>
                    <button>Test Coffee</button>
                </div>
                <div class="playbtn">
                    <button>
                        <img :src="playbtn" alt="" />
                    </button>
                    <p>Play video</p>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
section {
    background-image: url(../assets/images/mainbgimg.jpg);
    background-repeat: no-repeat;
    background-position: center center;
}
h1 {
    font-size: 72px;
    font-family: R-Regular;
    line-height: 130%;
    color: white;
    margin: 0;
}
.content p {
    font-family: U-Medium;
    font-size: 20px;
    color: rgba(255, 255, 255, 0.8);
    line-height: 180%;
    margin: 32px 0 64px;
}
.content button {
    width: 202px;
    height: 70px;
    background-color: #c99e71;
    font-family: I-Bold;
    font-size: 18px;
    color: #ffffff;
    text-transform: uppercase;
}
.wrapper {
    display: flex;
    padding-top: 272px;
    height: 864px;
    justify-content: space-between;
}
.content {
    max-width: 529px;
    width: 100%;
}
.playbtn {
    display: flex;
    flex-direction: column;
    align-items: center;
    gap: 20px;
    margin-top: 325px;
}
.playbtn button {
    border-radius: 100%;
    width: 70px;
    height: 70px;
    background-color: transparent;
    border: 1.5px solid #ffffff;
}
.playbtn p {
    font-family: I-Regular;
    font-size: 16px;
    color: #ffffff;
    text-transform: uppercase;
}
@media only screen and (max-width: 1335px) {
    .playbtn {
        margin-top: 275px;
        margin-right: 40px;
    }
}
@media only screen and (max-width: 1070px) {
    .playbtn {
        margin-top: 225px;
        margin-right: 30px;
    }
}
@media only screen and (max-width: 855px) {
    .playbtn {
        margin-top: 125px;
    }
    h1 {
        font-size: 52px;
    }
    .content p {
        font-size: 18px;
        margin: 26px 0 50px;
    }
    .content button {
        width: 192px;
        height: 65px;
        font-size: 17px;
    }
}
@media only screen and (max-width: 750px) {
    .wrapper {
        flex-direction: column;
        padding-top: 232px;
        align-items: center;
        text-align: center;
        height: 864px;
        justify-content: center;
        gap: 50px;
    }
    .playbtn {
        margin-top: 0;
        margin-right: 0;
    }
    .content button {
        width: 172px;
        height: 60px;
        font-size: 17px;
    }
    .playbtn button {
        width: 60px;
        height: 60px;
    }
    .playbtn p {
        font-size: 15px;
    }
}
@media only screen and (max-width: 590px) {
    .wrapper {
        padding-top: 182px;
    }
    h1 {
        font-size: 36px;
    }
    .content p {
        font-size: 15px;
        margin: 18px 0 40px;
    }
    .content button {
        width: 152px;
        height: 50px;
        font-size: 14px;
    }
    .playbtn button {
        width: 45px;
        height: 45px;
    }
    .playbtn p {
        font-size: 14px;
    }
}
</style>
