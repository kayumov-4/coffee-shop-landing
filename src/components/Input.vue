<script setup>
import arrowleft from "../assets/icons/arrow-left.svg";
import logo from "../assets/icons/logo.svg";
</script>

<template>
    <section>
        <div class="container">
            <div class="wrapper">
                <nav>
                    <img :src="logo" alt="" />
                    <ul>
                        <li><a href="">Home</a></li>
                        <li><a href="">Reservation</a></li>
                        <li><a href="">Menu</a></li>
                        <li><a href="">About</a></li>
                        <li><a href="">Pages</a></li>
                        <li><a href="">Shop</a></li>
                        <li><a href="">Blogs</a></li>
                    </ul>
                </nav>
                <div class="inputwrapper">
                    <input type="text" placeholder="Enter your email" />
                    <button>
                        <img :src="arrowleft" alt="" />
                    </button>
                </div>
            </div>
        </div>
    </section>
</template>
<style scoped>
ul {
    margin: 0;
    padding: 0;
}
.wrapper {
    display: flex;
    justify-content: space-between;
    align-items: center;
}
nav {
    display: flex;
    align-items: center;
    gap: 36px;
}
ul {
    display: flex;
    align-items: center;
    gap: 40px;
}
a {
    font-family: I-Regular;
    color: white;
    font-size: 20px;
}
.inputwrapper {
    width: 328px;
    height: 72px;
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 12px;
    padding: 12px;
    background-color: #1c1814;
    border-radius: 36px;
}
input {
    background-color: transparent;
    padding: 0 16px;
    color: #fff;
}
button {
    background-color: #c99e71;
    height: 48px;
    width: 48px;
    border-radius: 100%;
}
button img {
    transform: rotate(180deg);
}
@media only screen and (max-width: 1190px) {
    .wrapper {
        flex-direction: column;
        gap: 35px;
        justify-content: space-evenly;
    }
    a {
        font-size: 18px;
    }
    nav {
        flex-direction: column;
    }
    .inputwrapper {
        width: 620px;
        height: 72px;
    }
}
@media only screen and (max-width: 740px) {
    .wrapper {
        flex-direction: column;
        gap: 30px;
        justify-content: space-evenly;
    }
    nav {
        flex-direction: column;
    }
    a {
        font-size: 17px;
    }
    ul {
        gap: 30px;
    }
    .inputwrapper {
        width: 100%;
        height: 72px;
    }
}
@media only screen and (max-width: 635px) {
    .wrapper {
        flex-direction: column;
        gap: 20px;
        justify-content: space-evenly;
    }

    a {
        font-size: 17px;
    }
    ul {
        display: none;
    }
}

@media only screen and (max-width: 370px) {
    button {
        min-width: 48px;
    }
    input {
        width: 100%;
    }
}
</style>
