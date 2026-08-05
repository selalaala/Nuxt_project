<template>
    <div>
        <Navbar />
        <PageBanner title="Produk Comparison" />
        <ProdukComparison :comparison="comparison" />
        <General />
        <Quality />
        <Footer />
    </div>
</template>

<script setup>
import comparisons from '../../../data/produkcomparison.json'

const route = useRoute()

const comparison = comparisons.find(
  item => item.id === Number(route.params.id)
)
</script>