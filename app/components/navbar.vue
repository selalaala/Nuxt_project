<template>
  <nav class="navbar navbar-expand-lg bg-white shadow-sm py-3">
    <div class="container">
      <div class="navbar-brand d-flex align-items-center">
        <img src="../assets/svg/logo.svg" alt="logo"  />
        <h2>Furniro</h2>
      </div>

      <button
        class="navbar-toggler"
        type="button"
        data-bs-toggle="collapse"
        data-bs-target="#navbarNav">
        <span class="navbar-toggler-icon"></span>
      </button>


      <div class="collapse navbar-collapse" id="navbarNav">
           <ul class="navbar-nav mx-auto">
          <li class="nav-item">
            <a class="nav-link mx-3" href="#">Home</a>
          </li>

          <li class="nav-item">
            <a class="nav-link mx-3" href="#">Shop</a>
          </li>

          <li class="nav-item">
            <a class="nav-link mx-3" href="#">About</a>
          </li>

          <li class="nav-item">
            <a class="nav-link mx-3" href="#">Contact</a>
          </li>
        </ul>
        </div>


      <div class="nav-icon d-flex align-items-center gap-4">      
        <img src="../assets/svg/icon-user.svg" alt="user" />
        <img src="../assets/svg/icon-search.svg" alt="search" />
        <img src="../assets/svg/icon-hati.svg" alt="hati" />
        <img src="../assets/svg/keranjang.svg" alt="keranjang" />
      </div>  
    </div>
    </nav>
</template>

<script setup>
import '~/assets/css/navbar.css'
</script>