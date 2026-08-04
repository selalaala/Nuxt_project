<template>
    <div>
        <Navbar />
        <Sofa />
        <Deskripsi />
        <ProductSection   :showHeading="true" :products="products" :showButton="true"/>
        <Footer />
    </div>
</template>

<script setup>
const products = [
  {
    id: 1,
    image: '/svg/syltherine.svg',
    name: "Syltherine",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 2,
    image: '/svg/leviosa.svg',
    name: "Leviosa",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 3,
    image: '/svg/lolita.svg',
    name: "Lolita",
    desc: "Luxury big sofa",
    price: "Rp 7.000.000"
  },
  {
    id: 4,
    image: '/svg/respira.svg',
    name: "Respira",
    desc: "Outdoor bar table and stool",
    price: "Rp 500.000"
  }
]
</script>
