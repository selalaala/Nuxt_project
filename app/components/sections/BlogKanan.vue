<template>
  <section>
    <div class="mb-5">
      <input type="text" class="form-control" placeholder="Search">
    </div>
    <div class="mb-5">
      <h5 class="mb-4">Categories</h5>
      <div class="d-flex justify-content-between mb-3" v-for="item in categories" :key="item.id">
        <p class="mb-0">{{ item.name }}</p>
        <small>{{ item.total }}</small>
      </div>
    </div>

    <div>
      <h5 class="mb-4">Recent Posts</h5>
      <div class="d-flex gap-3 mb-4" v-for="post in recentPosts" :key="post.id">
        <img :src="post.image" width="80" class="rounded">
        <div>
          <p class="mb-1">{{ post.title }}</p>
          <small>{{ post.date }}</small>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
defineProps({
 categories : Array,
 recentPosts : Array
})
</script>