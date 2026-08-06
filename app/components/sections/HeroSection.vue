<template>
  <section class="hero">
    <div class="container h-100">      
      <div class="row h-100 justify-content-end align-items-center">
        <div class="col-lg-5">
          <div class="card hero-card border-0">
            <div class="card-body">
              <small>New Arrival</small>
              <h1 class="hero-tittle">Discover Our <br> New Collection</h1>
              <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Ut elit tellus, luctus nec ullamcorper mattis.</p>
              <button class="btn btn-furniro"><NuxtLink to="/shop" class="text-white text-decoration-none">Buy Now</NuxtLink></button>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero {
    background:url('/svg/background-discover.svg') ;
    min-height: 700px;
}

.card {
    top: 200px;
    background-color: #FFF3E3;
    padding: 20px 20px;
}

.hero-tittle {
    color: #B88E2F;
}

.btn-furniro{
    background-color: #B88E2F;
    color: white;
}

.btn-furniro:hover{
    background-color: #a67d25;
}
</style>
