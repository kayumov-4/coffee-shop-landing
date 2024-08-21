<script setup>
import logo from "../assets/icons/logo.svg";
import search from "../assets/icons/search.svg";
import shoppingbag from "../assets/icons/shopping-bag.svg";
import menu from "../assets/icons/menu.svg";
</script>

<template>
    <header>
        <div class="header-container">
            <nav>
                <ul class="left-ul">
                    <li><a href="">Home</a></li>
                    <li><a href="">About</a></li>
                    <li><a href="">Menu</a></li>
                    <li><a href="">Reservation</a></li>
                </ul>

                <img class="menu" :src="menu" alt="" />
                <img class="logo" :src="logo" alt="" />
                <ul class="right">
                    <li><a href="">Pages</a></li>
                    <li><a href="">Shop</a></li>
                    <li><a href="">Contact</a></li>
                    <li><img :src="search" alt="" /></li>
                    <li><img :src="shoppingbag" alt="" /></li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<style scoped>
header {
    background: #1c1814;
    position: fixed;
    top: 0;
    width: 100%;
    z-index: 1000;
}
.menu {
    display: none;
}
.header-container {
    max-width: 1360px;
    padding: 0 20px;
    margin: 0 auto;
}
nav {
    height: 125px;
    display: flex;
    align-items: center;
    justify-content: space-between;
}

.left-ul {
    display: flex;
    max-width: 397px;
    width: 100%;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 0;
}
.logo {
    margin-right: 72px;
}
.right {
    display: flex;
    max-width: 417px;
    width: 100%;
    align-items: center;
    justify-content: space-between;
    margin-bottom: 0;
}
a {
    color: white;
}
@media only screen and (max-width: 1160px) {
    .logo {
        margin-right: 0;
    }
}
@media only screen and (max-width: 960px) {
    .menu {
        display: block;
    }
    .left-ul {
        display: none;
    }
    .right {
        max-width: 500px;
    }
    nav {
        gap: 40px;
    }
}
@media only screen and (max-width: 460px) {
    .right a {
        display: none;
    }

    nav {
        gap: 20px;
    }
}
</style>
