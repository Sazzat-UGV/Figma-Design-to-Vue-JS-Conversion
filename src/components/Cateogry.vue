<template>
  <section id="category" class="flex flex-col items-center py-32">
    <h2 class="my-10 text-5xl md:text-6xl font-bold text-white">Category</h2>
    <div class="grid grid-cols-1 md:grid-cols-3 place-items-center">
      <div
        class="text-white grid place-items-center gap-5 text-center"
        v-for="category of categories"
        :key="category.id"
      >
        <div class="p-10">
          <img :src="category.image" alt="category-image" class="w-full" />
        </div>
        <h3 class="text-3xl font-bold">{{ category.title }}</h3>
        <p class="w-3/4">{{ category.description }}</p>
      </div>
    </div>
  </section>
</template>
<script setup>
import { ref } from "vue";
import category1 from "../assets/images/category/category1-img.webp";
import category2 from "../assets/images/category/category2-img.webp";
import category3 from "../assets/images/category/category3-img.webp";

const categories = ref([
  {
    id: 1,
    title: "Ghost",
    image: category1,
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.",
  },
  {
    id: 2,
    title: "Witch",
    image: category2,
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.",
  },
  {
    id: 3,
    title: "Pumpkin",
    image: category3,
    description:
      "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Id id consequat, eu faucibus nulla. Ultrices mattis lacus, sed maecenas nascetur.",
  },
]);
</script>
