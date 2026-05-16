<script setup>
import Feature from './components/Feature.vue';
import Hero from './components/Hero.vue';
import NavBar from './components/NavBar.vue'
import Productive from './components/Productive.vue';
import FAQ from './components/FAQ.vue';
import Testimonial from './components/Testimonial.vue';
import EarlyAccess from './components/EarlyAccess.vue'
import Footer from './components/Footer.vue'
</script>

<template>
    <div class=" dark:text-white dark:bg-darkBlue">
        <NavBar/>
        <Hero/>
        <Feature/>
        <Productive/>
        <FAQ/>
        <Testimonial/>
        <EarlyAccess/>
        <Footer/>
    </div>
</template>
