<template>
  <section class="py-3">
    <div class="container">
      <div class="row g-5">
        <div class="col-lg-6">
          <div class="row">
            <div class="col-2">
              <div class="d-flex flex-column gap-3">
                <div v-for="(image, index) in detailproduk.gallery" :key="index">
                  <img :src="image" class="img-fluid">
                </div>
              </div>
            </div>

            <div class="col-10">
              <div class="text-center">
                <img :src="detailproduk.image" class="img-fluid">
              </div>
            </div>
          </div>
        </div>

        <div class="col-lg-6">
          <h1 class="fw-normal mb-2">
            {{ detailproduk.name }}
          </h1>
          <h4 class="text-secondary mb-3">
            {{ detailproduk.price }}
          </h4>
          <div class="d-flex align-items-center gap-3 mb-3">
            <div class="text-warning">
              <i v-for="n in Math.floor(detailproduk?.rating || 0)" :key="n" class="bi bi-star-fill"></i>
              <i v-if="detailproduk?.rating && detailproduk.rating % 1 !== 0" class="bi bi-star-half"></i>
            </div>

            <div class="vr"></div>
            <small class="text-secondary">
              {{ detailproduk.review }}
            </small>
          </div>
          <p class="text-secondary">
            {{ detailproduk.description }}
          </p>
          <small class="text-secondary">
            Size
          </small>
          <div class="d-flex gap-2 mt-2 mb-4">
            <button v-for="size in detailproduk.size" :key="size" class="btn btn-light btn-sm border">
              {{ size }}
            </button>
          </div>
          <small class="text-secondary">
            Color
          </small>
          <div class="d-flex gap-3 mt-2 mb-4">
            <span v-for="color in detailproduk.colors" :key="color" class="rounded-circle color-dot" :style="{ backgroundColor: color }"></span>
          </div>

          <div class="d-flex flex-wrap gap-3">
            <div class="border rounded d-flex align-items-center px-3 py-2">
              <button class="btn btn-sm">-</button>
              <span class="mx-3">1</span>
              <button class="btn btn-sm">+</button>
            </div>
            <NuxtLink to="/cart" class="btn btn-outline-dark px-4 py-3">
              Add To Cart
            </NuxtLink>
            <NuxtLink :to="`/produkcomparison/${detailproduk.id}`" class="btn btn-outline-dark px-4 py-3">
              + Compare
            </NuxtLink>
          </div>

          <hr class="my-5">
          <table class="table table-borderless text-secondary">
            <tbody>
              <tr>
                <td width="120">SKU</td>
                <td>: {{ detailproduk.sku }}</td>
              </tr>
              <tr>
                <td>Category</td>
                <td>: {{ detailproduk.category }}</td>
              </tr>
              <tr>
                <td>Tags</td>
                <td>: {{ detailproduk.tags }}</td>
              </tr>
              <tr>
                <td>Share</td>
                <td>
                  <i class="bi bi-facebook me-3"></i>
                  <i class="bi bi-linkedin me-3"></i>
                  <i class="bi bi-twitter-x"></i>
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.btn-default {
    border-color: black;
}

.bg-furniro{
    background:#B88E2F;
}

.color-dot{
    width:30px;
    height:30px;
    display:inline-block;
}

@media (max-width: 991px){
    section{
        padding-top: 10px !important;
    }
}
</style>

<script setup>
defineProps({
  detailproduk: Object
})
</script>