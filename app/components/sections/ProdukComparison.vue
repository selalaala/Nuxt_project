<template>
    <section class="product-comparison">
        <div class="container px-lg-5 px-md-4 px-3">
            <div class="row gx-4 gy-4 align-items-start">
                <div class="col-xl-3 col-lg-3 col-md-6">
                    <h2>Go to Product page for more Products</h2>
                    <button class="btn btn-link text-secondary">View More</button>
                </div>
               <div class="col-xl-3 col-lg-3 col-md-6">
                <img :src="comparison.leftProduct.image">
                <div>
                    <h5>{{ comparison.leftProduct.name }}</h5>
                    <small>{{ comparison.leftProduct.price }}</small>
                    <div>
                        <small>{{ comparison.leftProduct.rating }}</small>
                        <i v-for="n in comparison.leftProduct.stars" :key="n" class="bi bi-star-fill text-warning"> </i>
                        <i v-if="comparison.leftProduct.halfStar" class="bi bi-star-half text-warning"></i>
                    </div>
                </div>
            </div>

            <div class="col-xl-3 col-lg-3 col-md-6">
                <img :src="comparison.rightProduct.image">
                <div>
                    <h5>{{ comparison.rightProduct.name }}</h5>
                    <small>{{ comparison.rightProduct.price }}</small>
                    <div>
                        <small>{{ comparison.rightProduct.rating }}</small>
                        <i v-for="n in comparison.rightProduct.stars" :key="n" class="bi bi-star-fill text-warning"></i>
                        <i v-if="comparison.rightProduct.halfStar" class="bi bi-star-half text-warning"></i>
                    </div>
                </div>
            </div>
                <div class="col-xl-3 col-lg-3 col-md-6">
                    <h3>Add a Product</h3>
                    <div class="dropdown">
                        <button class="btn btn-furniro dropdown-toggle" type="button" data-toggle="dropdown">Dropdown
                            <span class="caret"></span>
                        </button>
                            <ul class="dropdown-menu">
                                <li><a href="#"></a></li>
                                <li><a href="#"></a></li>
                                <li><a href="#"></a></li>
                            </ul>
                        </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
@media (min-width: 992px) and (max-width: 1399px) {

  .product-comparison .row {
    --bs-gutter-x: 2rem; 
  }

  .product-comparison h2 {
    font-size: 28px;
  }

  .product-comparison h5 {
    font-size: 16px;
  }

  .product-comparison img {
    width: 100%;
    max-width: 180px;
    height: auto;
  }

  .product-comparison .col-lg-3 {
    padding-left: 12px;
    padding-right: 12px;
  }

  .compare-select {
    width: 100%;
  }
}
</style>
<script setup>
defineProps({
  comparison: Object
})
</script>