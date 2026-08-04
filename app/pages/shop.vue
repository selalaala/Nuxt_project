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

const products = [
{
  id:1,
  image:"/svg/syltherine.svg",
  name:"Syltherine",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"Rp 3.500.000",
  badge:"-30%",
  badgeColor:"discount"
},
{
  id:2,
  image:"/svg/leviosa.svg",
  name:"Leviosa",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"",
  badge:"",
  badgeColor:""
},
{
  id:3,
  image:"/svg/lolita.svg",
  name:"Lolita",
  desc:"Luxury big sofa",
  price:"Rp 7.000.000",
  oldPrice:"Rp 14.000.000",
  badge:"-50%",
  badgeColor:"discount"
},
{
  id:4,
  image:"/svg/respira.svg",
  name:"Respira",
  desc:"Outdoor bar table and stool",
  price:"Rp 500.000",
  oldPrice:"",
  badge:"New",
  badgeColor:"new"
},
{
  id:1,
  image:"/svg/syltherine.svg",
  name:"Syltherine",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"Rp 3.500.000",
  badge:"-30%",
  badgeColor:"discount"
},
{
  id:2,
  image:"/svg/leviosa.svg",
  name:"Leviosa",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"",
  badge:"",
  badgeColor:""
},
{
  id:3,
  image:"/svg/lolita.svg",
  name:"Lolita",
  desc:"Luxury big sofa",
  price:"Rp 7.000.000",
  oldPrice:"Rp 14.000.000",
  badge:"-50%",
  badgeColor:"discount"
},
{
  id:4,
  image:"/svg/respira.svg",
  name:"Respira",
  desc:"Outdoor bar table and stool",
  price:"Rp 500.000",
  oldPrice:"",
  badge:"New",
  badgeColor:"new"
},
{
  id:1,
  image:"/svg/syltherine.svg",
  name:"Syltherine",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"Rp 3.500.000",
  badge:"-30%",
  badgeColor:"discount"
},
{
  id:2,
  image:"/svg/leviosa.svg",
  name:"Leviosa",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"",
  badge:"",
  badgeColor:""
},
{
  id:3,
  image:"/svg/lolita.svg",
  name:"Lolita",
  desc:"Luxury big sofa",
  price:"Rp 7.000.000",
  oldPrice:"Rp 14.000.000",
  badge:"-50%",
  badgeColor:"discount"
},
{
  id:4,
  image:"/svg/respira.svg",
  name:"Respira",
  desc:"Outdoor bar table and stool",
  price:"Rp 500.000",
  oldPrice:"",
  badge:"New",
  badgeColor:"new"
},
{
  id:1,
  image:"/svg/syltherine.svg",
  name:"Syltherine",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"Rp 3.500.000",
  badge:"-30%",
  badgeColor:"discount"
},
{
  id:2,
  image:"/svg/leviosa.svg",
  name:"Leviosa",
  desc:"Stylish cafe chair",
  price:"Rp 2.500.000",
  oldPrice:"",
  badge:"",
  badgeColor:""
},
{
  id:3,
  image:"/svg/lolita.svg",
  name:"Lolita",
  desc:"Luxury big sofa",
  price:"Rp 7.000.000",
  oldPrice:"Rp 14.000.000",
  badge:"-50%",
  badgeColor:"discount"
},
{
  id:4,
  image:"/svg/respira.svg",
  name:"Respira",
  desc:"Outdoor bar table and stool",
  price:"Rp 500.000",
  oldPrice:"",
  badge:"New",
  badgeColor:"new"
}
]
</script>