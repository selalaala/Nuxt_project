<template>
    <div>
        <Navbar />
        <Breakcrumb :title="detailprodukItem.name" />
        <Sofa :detailproduk="detailprodukItem"/>
        <Deskripsi />
        <ProductSection :showHeading="true" :products="sofaProducts" :showButton="true"/>
        <Footer />
    </div>
</template>

<script setup>
import products from '../../../data/Product.json'
const sofaProducts = products.slice(0, 4)

import detailproduk from '../../../data/detailproduk.json'
const route = useRoute()
const detailprodukItem = detailproduk.find(
  item => item.id === Number(route.params.id)
)
</script>
