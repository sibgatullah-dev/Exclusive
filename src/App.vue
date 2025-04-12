<template>
<Nav></Nav>
<router-view></router-view>

<Footer></Footer>
</template>

<script setup>
import Nav from '../src/components/Nav.vue';
import Footer from '../src/components/Footer.vue';
import Homepage from './pages/Homepage.vue';
</script>