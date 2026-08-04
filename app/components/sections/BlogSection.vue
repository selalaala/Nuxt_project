<template>
  <section>
    <BlogCard v-for="item in blogs":key="item.id":blog="item"/>
  </section>
</template>

<script setup>
import BlogCard from '~/components/cards/BlogCard.vue'
defineProps({
  blogs: Array
})
</script>