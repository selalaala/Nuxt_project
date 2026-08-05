<template>
    <div>
        <Navbar />
        <PageBanner title="Cart" />
        <Cart :cartItems="cartItems" :cartSummary="cartSummary" />
        <Quality />
        <Footer />
    </div>
</template>

<script setup>
import cartItems from '../../data/Cart.json'
import cartSummary from '../../data/CartSummary.json'
</script>