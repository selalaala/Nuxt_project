<template>
  <div class="col-lg-3 col-md-6 mb-4">
    <div class="product-item">
      <img :src="product.image" class="product-image" alt="" />
      <div v-if="product.badge" class="badge-circle" :class="product.badgeColor">
        {{ product.badge }}
      </div>

      <div class="overlay">
        <button class="btn"><NuxtLink to="/cart" class="btn btn-cart">Add to Cart</NuxtLink></button>
        <div class="overlay-menu">
          <span><i class="bi bi-share"></i> <NuxtLink :to="`/sofa/${product.id}`"  class="btn-link text-light text-decoration-none">Share</NuxtLink> </span>
          <span><i class="bi bi-arrow-left-right">  </i><NuxtLink :to="`/produkcomparison/${product.id}`" class="btn-link text-light text-decoration-none">Compare</NuxtLink></span>
        </div>
      </div>
    </div>

    <div class="product-info">
      <h5>{{ product.name }}</h5>
      <small>{{ product.desc }}</small>
      <div class="price">
        <h6>{{ product.price }}</h6>
        <small v-if="product.oldPrice" class="old-price">
          {{ product.oldPrice }}
        </small>
      </div>
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

.btn-cart{
    color: #B88E2F;
    background-color: #fff;
    margin: 35px;
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

.badge-circle{
    position:absolute;
    top:20px;
    right:20px;
    width:48px;
    height:48px;
    border-radius:50%;
    display:flex;
    justify-content:center;
    align-items:center;
    color:white;
    font-size:14px;
    font-weight:600;
}

.discount{
    background:#E97171;
}

.new{
    background:#2EC1AC;
}

.price{
    display:flex;
    align-items:center;
    gap:10px;
}

.old-price{
    color:#B0B0B0;
    text-decoration:line-through;
}
</style>