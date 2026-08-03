<template>
  <section>
    <div class="row text-center" v-if="showHeading">
      <h3>Our Products</h3>
    </div>
    <div class="container">
      <div class="row">
        <ProductCard v-for="item in products" :key="item.id" :product="item"/>
      </div>
      <div class="text-center mt-4" v-if="showButton">
        <button class="btn btn-outline-primary btn-show"><NuxtLink to="/shop">Show More</NuxtLink></button>
      </div>
    </div>
  </section>
</template>

<script setup>
import ProductCard from './ProductCard.vue'
defineProps({
  products: Array,
  showHeading: Boolean,
  showButton: Boolean
})
</script>