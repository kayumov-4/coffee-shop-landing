<script setup>
import "./style.css";
import Header from "./components/Header.vue";
import First from "./components/First.vue";
import Coffees from "./components/Coffees.vue";
import OurHistory from "./components/OurHistory.vue";
import PopularProduct from "./components/PopularProduct.vue";
import CoffeMachine from "./components/CoffeMachine.vue";
import Menu from "./components/Menu.vue";
import CTestimonial from "./components/CTestimonial.vue";
import Reservation from "./components/Reservation.vue";
import OurTestimonial from "./components/OurTestimonial.vue";
import Input from "./components/Input.vue";
import Footer from "./components/Footer.vue";
</script>

<template>
    <Header />
    <main>
        <First />
        <Coffees />
        <OurHistory />
        <PopularProduct />
        <CoffeMachine />
        <Menu />
        <CTestimonial />
        <Reservation />
        <OurTestimonial />
        <Input />
    </main>
    <Footer />
</template>

<style scoped></style>
