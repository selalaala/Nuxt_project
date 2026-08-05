<template>
  <div>
     <Navbar />
     <HeroSection />
     <Browse :browses="browses" />
     <ProductSection   :showHeading="true" :products="products" :showButton="true"/>
     <Room-inspiration />
     <Furniture :furnitures="furnitures"/>
     <Footer />
  </div>
</template>

<script setup>
import products from '../../data/Product.json'
import browses from '../../data/Browse.json'
import furnitures from '../../data/Furniture.json'
</script>
