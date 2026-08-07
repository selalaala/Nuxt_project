<template>
  <nav class="navbar navbar-expand-lg bg-white shadow-sm py-3">
    <div class="container">
      <div class="navbar-brand d-flex align-items-center">
        <img src="/svg/logo.svg" alt="logo" />
        <h2>Furniro</h2>
      </div>
      <div class="collapse navbar-collapse d-none d-lg-flex">
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

      <div class="nav-right d-flex align-items-center">
        <button class="cart-btn" type="button" @click="cartOpen = true">
          <img src="/svg/keranjang.svg" alt="keranjang" />
        </button>
        <button class="navbar-toggler d-lg-none" type="button" @click="menuOpen = true">
          <span class="navbar-toggler-icon"></span>
        </button>
      </div>
    </div>
  </nav>

 
  <div class="cart-overlay" v-if="menuOpen" @click="menuOpen=false"></div>
  <div class="menu-sidebar" :class="{show: menuOpen}">
    <div class="d-flex justify-content-between align-items-center mb-4">
      <h5>Menu</h5>
      <img src="/svg/close.svg" class="close-icon" @click="menuOpen=false"/>
    </div>
    <NuxtLink to="/" class="nav-link" @click="menuOpen=false">Home</NuxtLink>
    <NuxtLink to="/shop" class="nav-link" @click="menuOpen=false"> Shop</NuxtLink>
    <NuxtLink to="/blog" class="nav-link" @click="menuOpen=false">Blog</NuxtLink>
    <NuxtLink to="/contact" class="nav-link" @click="menuOpen=false">Contact</NuxtLink>
  </div>

  <div class="cart-overlay" v-if="cartOpen" @click="cartOpen = false"></div>
  <div class="cart-sidebar" :class="{ show: cartOpen }">
    <div>
      <div class="d-flex justify-content-between align-items-center">
        <h5>Shopping Cart</h5>
        <img src="/svg/close.svg" class="close-icon" @click="cartOpen = false" />
      </div>
      <hr>
    </div>
    <div class="cart-items">
      <div class="d-flex align-items-center mb-3">
        <img src="/svg/sofa.svg" width="70">
        <div class="ms-3">
          <h6>Asgaard Sofa</h6>
          <small>1 × Rp. 250,000.00</small>
        </div>
      </div>
      <div class="d-flex align-items-center mb-3">
        <img src="/svg/casaliving.svg" width="70">
        <div class="ms-3">
          <h6>Casaliving Wood</h6>
          <small>1 × Rp. 270,000.00</small>
        </div>
      </div>
    </div>
    <div class="cart-footer">
      <div class="d-flex justify-content-between mb-3">
        <span>Subtotal</span>
        <strong class="text-warning">Rp. 520,000.00</strong>
      </div>
      <hr>
      <div class="d-flex justify-content-between gap-2">
        <button @click="goToPage('/cart')" class="btn btn-outline-dark">Cart</button>
        <button @click="goToPage('/checkout')" class="btn btn-outline-dark">Checkout</button>
        <button @click="goToPage('/produkcomparison/1')" class="btn btn-outline-dark">Comparison</button>
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
const menuOpen = ref(false)
const goToPage = (path) => {
  cartOpen.value = false
  router.push(path)
}
</script>