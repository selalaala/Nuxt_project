<template>
  <div>
    <Navbar />
    <PageBanner title="Shop" />
    <ShopFilter />
    <ProductSection :showHeading="false" :products="shopProducts" :showButton="false"/>
    <Quality />
    <Footer />
  </div>
</template>

<script setup>
import products from '../../data/Product.json'

const firstFour = products.slice(0, 4)
const shopProducts = []
for (let i = 0; i < 4; i++) {
  shopProducts.push(...firstFour)
}
</script>