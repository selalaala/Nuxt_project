<template>
    <div>
        <Navbar />
        <PageBanner title="Blog" />
        <div class="container py-5">
            <div class="row">
                <div class="col-lg-8">
                    <BlogSection :blogs="blogs"/>
                </div>
                <div class="col-lg-4">
                    <BlogKanan />
                </div>
            </div>
        </div>
        <Quality />
        <Footer />
  </div>
</template>


<script setup>
import blog1 from '~/assets/svg/blog1.svg'
import blog2 from '~/assets/svg/blog2.svg'
import bloghandmade from '~/assets/svg/bloghandmade.svg'

const blogs = [
  {
    id:1,
    image: blog1,
    admin:"Admin",
    date:"14 Oct 2022",
    category:"Wood",
    title:"Going all-in with millennial design",
    desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Mus mauris vitae ultricies leo integer malesuada nunc. In nulla posuere sollicitudin aliquam ultrices. Morbi blandit cursus risus at ultrices mi tempus imperdiet. Libero enim sed faucibus turpis in. Cursus mattis molestie a iaculis at erat. Nibh cras pulvinar mattis nunc sed blandit libero. Pellentesque elit ullamcorper dignissim cras tincidunt. Pharetra et ultrices neque ornare aenean euismod elementum."
  },
  {
    id:2,
    image: blog2,
    admin:"Admin",
    date:"14 Oct 2022",
    category:"Wood",
    title:"Exploring new ways of decorating",
    desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Mus mauris vitae ultricies leo integer malesuada nunc. In nulla posuere sollicitudin aliquam ultrices. Morbi blandit cursus risus at ultrices mi tempus imperdiet. Libero enim sed faucibus turpis in. Cursus mattis molestie a iaculis at erat. Nibh cras pulvinar mattis nunc sed blandit libero. Pellentesque elit ullamcorper dignissim cras tincidunt. Pharetra et ultrices neque ornare aenean euismod elementum."
  },
  {
    id:3,
    image: bloghandmade,
    admin:"Admin",
    date:"14 Oct 2022",
    category:"Wood",
    title:"Handmade pieces that took time to make",
    desc:"Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Mus mauris vitae ultricies leo integer malesuada nunc. In nulla posuere sollicitudin aliquam ultrices. Morbi blandit cursus risus at ultrices mi tempus imperdiet. Libero enim sed faucibus turpis in. Cursus mattis molestie a iaculis at erat. Nibh cras pulvinar mattis nunc sed blandit libero. Pellentesque elit ullamcorper dignissim cras tincidunt. Pharetra et ultrices neque ornare aenean euismod elementum."
  }
]
</script>