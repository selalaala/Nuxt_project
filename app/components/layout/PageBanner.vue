<template>
  <section class="banner">
    <div class="overlay">
      <img src="/svg/logo.svg" alt="Logo" class="logo" />
      <h1>{{ title }}</h1>
      <p>Home > {{ title }}</p>
    </div>
  </section>
</template>

<script setup>
defineProps({
  title: {
    type: String,
    default: "Home"
  }
})
</script>

<style scoped>
.banner {
  background: url('/svg/shop.svg') center/cover no-repeat;
  height: 300px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.overlay {
  text-align: center;
}

.logo {
  width: 60px;
  margin-bottom: 10px;
}

h1 {
  font-size: 40px;
  margin: 10px 0;
}

p {
  font-size: 16px;
}
</style>