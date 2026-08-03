<template>
  <div>
    <Navbar />
    <PageBanner title="Shop" />
    <ShopFilter />
    <ProductSection :showHeading="false" :products="products" :showButton="false"/>
    <Quality />
    <Footer />
  </div>
</template>

<script setup>
import syltherine from '~/assets/svg/syltherine.svg'
import leviosa from '~/assets/svg/leviosa.svg'
import lolita from '~/assets/svg/lolita.svg'
import respira from '~/assets/svg/respira.svg'

const products = [
  {
    id: 1,
    image: syltherine,
    name: "Syltherine",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 2,
    image: leviosa,
    name: "Leviosa",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 3,
    image: lolita,
    name: "Lolita",
    desc: "Luxury big sofa",
    price: "Rp 7.000.000"
  },
  {
    id: 4,
    image: respira,
    name: "Respira",
    desc: "Outdoor bar table and stool",
    price: "Rp 500.000"
  },
  {
    id: 1,
    image: syltherine,
    name: "Syltherine",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 2,
    image: leviosa,
    name: "Leviosa",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 3,
    image: lolita,
    name: "Lolita",
    desc: "Luxury big sofa",
    price: "Rp 7.000.000"
  },
  {
    id: 4,
    image: respira,
    name: "Respira",
    desc: "Outdoor bar table and stool",
    price: "Rp 500.000"
  },
  {
    id: 1,
    image: syltherine,
    name: "Syltherine",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 2,
    image: leviosa,
    name: "Leviosa",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 3,
    image: lolita,
    name: "Lolita",
    desc: "Luxury big sofa",
    price: "Rp 7.000.000"
  },
  {
    id: 4,
    image: respira,
    name: "Respira",
    desc: "Outdoor bar table and stool",
    price: "Rp 500.000"
  },
  {
    id: 1,
    image: syltherine,
    name: "Syltherine",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 2,
    image: leviosa,
    name: "Leviosa",
    desc: "Stylish cafe chair",
    price: "Rp 2.500.000"
  },
  {
    id: 3,
    image: lolita,
    name: "Lolita",
    desc: "Luxury big sofa",
    price: "Rp 7.000.000"
  },
  {
    id: 4,
    image: respira,
    name: "Respira",
    desc: "Outdoor bar table and stool",
    price: "Rp 500.000"
  },

]
</script>