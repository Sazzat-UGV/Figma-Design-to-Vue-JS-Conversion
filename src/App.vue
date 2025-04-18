<template>
<div class="container overflow-x-hidden">
<Navbar/>
<Home/>
<Category/>
<TrickOrTreat/>
</div>
</template>

<script setup>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue';
import Category from './components/Cateogry.vue';
import TrickOrTreat from './components/TrickOrTreat.vue';
</script>