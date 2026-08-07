<template>
  <section class="py-5">
    <div class="container">
      <div class="card border-0 p-4">
        <div class="row align-items-center">
          <div class="col-lg-6 text-center mb-4 mb-lg-0">
            <img :src="blog.image" :alt="blog.name" class="img-fluid rounded">
          </div>
          <div class="col-lg-6">
            <h2 class="mb-3">
              {{ blog.name }}
            </h2>
            <div class="d-flex flex-wrap gap-3 text-secondary mb-3">
              <span><i class="bi bi-person me-1"></i>{{ blog.admin }}</span>
              <span><i class="bi bi-calendar3 me-1"></i>{{ blog.date }}</span>
              <span><i class="bi bi-tag me-1"></i>{{ blog.category }}</span>
            </div>
            <p class="text-secondary lh-lg">
              {{ blog.description }}
            </p>
          </div>
          <div class="mt-4">
            <p class="text-secondary lh-lg">
                {{ blog.description2 }}
            </p>
        </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
defineProps({
  blog: Object
})
</script>