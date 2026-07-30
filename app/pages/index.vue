<template>
  <div>
     <Navbar />
     <HeroSection />
     <Browse />
     <ProductSection   :showHeading="true" :products="products" :showButton="true"/>
     <Room-inspiration />
     <Furniture />
     <Footer />
  </div>
</template>

<script setup>
import syltherine from '~/assets/svg/syltherine.svg'
import leviosa from '~/assets/svg/leviosa.svg'
import lolita from '~/assets/svg/lolita.svg'
import respira from '~/assets/svg/respira.svg'
import grifo from '~/assets/svg/gripo.svg'
import muggo from '~/assets/svg/muggo.svg'
import pinky from '~/assets/svg/pinky.svg'
import potty from '~/assets/svg/potty.svg'

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
    id: 5,
    image: grifo,
    name: "Grifo",
    desc: "Night lamp",
    price: "Rp 1.500.000"
  },
  {
    id: 6,
    image: muggo,
    name: "Muggo",
    desc: "Small mug",
    price: "Rp 150.000"
  },
  {
    id: 7,
    image: pinky,
    name: "Pinky",
    desc: "Cute bed set",
    price: "Rp 7.000.000"
  },
  {
    id: 8,
    image: potty,
    name: "Potty",
    desc: "Minimalist flower pot",
    price: "Rp 500.000"
  }
]
</script>
