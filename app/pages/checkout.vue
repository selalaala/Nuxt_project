<template>
    <div>
        <Navbar />
        <PageBanner title="Checkout" />
        <Checkout :checkout="checkout" />
        <Quality />
        <Footer />
    </div>
</template>

<script setup>  
import checkout from '../../data/Checkout.json'
</script>