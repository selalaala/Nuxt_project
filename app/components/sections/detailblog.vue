<template>
    <section>
        <div class="container">
            <div class="blog-detail" v-for="blog in blogs" :key="blog.id" :blog="blog">
                <h1>{{ blog.name }}</h1>
                <img :src="blog.image" class="img-fluid" :alt="blog.name">
                <p class="mt-4">{{ blog.description }}</p>
            </div>
        </div>
    </section>
</template>

<script setup>
defineProps({
  blog: Object
})
</script>