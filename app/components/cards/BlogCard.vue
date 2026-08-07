<template>
  <div class="mb-5">
    <img :src="blog.image" class="img-fluid rounded">
    <div class="d-flex align-items-center gap-4 mt-3">       
        <i class="bi bi-person"></i>
        <small>{{ blog.admin }}</small>
        <i class="bi bi-calendar3"></i>
        <small class="mx-2">{{ blog.date }}</small>
        <i class="bi bi-tag"></i>
        <small>{{ blog.category }}</small>
    </div>
    <h3 class="mt-3">{{ blog.title }}</h3>
    <p class="text-secondary">{{ blog.desc }}</p>
    <button class="btn btn-link"><NuxtLink :to="`/blog/${blog.id}`" class="text-black">Read More</NuxtLink></button>
  </div>
</template>

<script setup>
defineProps({
  blog: Object
})
</script>