<template>
  <nav class="navbar navbar-expand-lg bg-white shadow-sm py-3">
    <div class="container">
      <div class="navbar-brand d-flex align-items-center">
        <img src="../assets/svg/logo.svg" alt="logo"  />
        <h2>Furniro</h2>
      </div>

      <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>

      <div class="collapse navbar-collapse" id="navbarNav">
           <ul class="navbar-nav mx-auto">
            <li class="nav-item">
              <NuxtLink to="/" class="nav-link mx-3">Home</NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink to="/shop" class="nav-link mx-3">Shop</NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink to="/blog" class="nav-link mx-3">Blog</NuxtLink>
          </li>

          <li class="nav-item">
            <NuxtLink to="/contact" class="nav-link mx-3">Contact</NuxtLink>
          </li>
        </ul>
      </div>
      <div class="nav-icon d-flex align-items-center">
        <button class="cart-btn" type="button" @click="cartOpen = true">
          <img src="../assets/svg/keranjang.svg" alt="Keranjang" />
        </button>
      </div>
    </div>
    </nav>
  
    <div class="cart-overlay" v-if="cartOpen" @click="cartOpen = false"></div>
    <div class="cart-sidebar" :class="{ show: cartOpen }">
        <div class="offcanvas-header d-flex justify-content-between align-items-center">
        <h5>Shopping Cart</h5>
        <img src="../assets/svg/close.svg" alt="Close" class="close-icon" @click="cartOpen = false">
      </div>

      <div class="offcanvas-body">
         <div class="d-flex align-items-center justify-content-between mb-3">
          <img src="~/assets/svg/sofa.svg" width="70" class="rounded"/>
          <div class="flex-grow-1 ms-3">
            <h6 class="mb-1">Asgaard Sofa</h6>
            <small>1 × <span class="text-warning">Rp. 250,000.00</span></small>
          </div>
          <button type="button" class="close-btn" @click="cartOpen = false">
            <i class="bi bi-x-circle-fill"></i>  
          </button>
        </div>
         <div class="d-flex align-items-center justify-content-between mb-3">
          <img src="~/assets/svg/casaliving.svg" width="70" class="rounded"/>
          <div class="flex-grow-1 ms-3">
            <h6 class="mb-1">Casaliving Wood</h6>
            <small>1 × <span class="text-warning">Rp. 270,000.00</span></small>
          </div>
          <button type="button" class="close-btn" data-bs-dismiss="offcanvas">
            <i class="bi bi-x-circle-fill"></i>  
          </button>
        </div>

        <div class="d-flex justify-content-between mb-3">
          <span>Subtotal</span>
          <strong>Rp. 520,000.00</strong>
        </div>
        <hr>
        <div class="d-flex gap-3">
          <button @click="goToPage('/cart')" class="btn btn-outline-dark">Cart</button>
          <button @click="goToPage('/checkout')" class="btn btn-outline-dark">Checkout</button>
          <button @click="goToPage('/produk-comparison')" class="btn btn-outline-dark">Comparison</button>
        </div>
      </div>
    </div>
</template>

<script setup>
import '~/assets/css/navbar.css'
import { ref } from 'vue'
import { useRouter } from 'vue-router'

const router = useRouter()

const cartOpen = ref(false)

const goToPage = (path) => {
  cartOpen.value = false
  router.push(path)
}
</script>