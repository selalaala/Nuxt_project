<template>
  <section>
    <BlogCard v-for="item in blogs":key="item.id":blog="item"/>
  </section>
</template>

<script setup>
import BlogCard from './BlogCard.vue'

defineProps({
  blogs: Array
})
</script>