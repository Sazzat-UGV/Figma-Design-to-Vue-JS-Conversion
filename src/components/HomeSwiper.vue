<template>

</template>
<script setup>
import { Pagination } from 'swiper';
import { Swiper , SwiperSlide } from 'swiper/vue';
// import Swiper and modules styles
import 'swiper/css';
import 'swiper/css/navigation';

// init Swiper:
const swiper = new Swiper('.swiper', {
  // configure Swiper to use modules
  modules: [Navigation, Pagination],
  ...
});
</script>