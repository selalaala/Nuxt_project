<template>
  <div class="col-lg-3 col-md-6 mb-4">
    <div class="product-item">
      <img :src="product.image" class="product-image" alt="" />
      <div class="overlay">
      <button class="btn btn-light">Add to Cart</button>
      <div class="overlay-menu">
        <span><i class="bi bi-share"></i><NuxtLink to="/sofa">Share</NuxtLink> </span>
        <span><i class="bi bi-arrow-left-right"></i> Compare</span>
        <span><i class="bi bi-heart"></i> Like</span>
      </div>
    </div>
    </div>
    <div class="product-info">
        <h5>{{ product.name }}</h5>
        <small>{{ product.desc }}</small>
        <h6>{{ product.price }}</h6>
     </div>
  </div>
</template>

<script setup>
defineProps({
  product: Object
})
</script>

<style scoped>
.product-image {
  width: 100%;
  display: block;
}

.product-info {
  padding-top: 10px;
  background-color: #F4F5F7;
}

.product-info h5 {
  margin-bottom: 4px;
}

.product-info small {
  display: block;
  margin-bottom: 4px;
}

.product-item{
    width: 100%;
    position: relative;
}

.overlay{
    position: absolute;
    inset: 0;
    background: rgba(58,58,58,.72);
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    opacity: 0;
    transition: .3s;
}

.product-item:hover .overlay{
    opacity: 1;
}

.overlay-menu{
    display:flex;
    gap:20px;
    color:white;
    margin-top:20px;
}
</style>