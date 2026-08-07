<template>
  <section>
    <div class="container">
      <div class="row text-center">
        <h3>Browse The Range</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit.</p>
      </div>
    </div>

    <div class="container">
      <div class="row">
        <div class="col-lg-4 text-center" v-for="browse in browses" :key="browse.id">
          <img :src="browse.image" class="img-fluid" :alt="browse.name">
          <div class="card-body">
            <h5 class="text-center">{{ browse.name }}</h5>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
defineProps({
  browses: Array
})
</script>