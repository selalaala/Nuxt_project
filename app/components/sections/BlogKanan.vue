<template>
  <section>
    <div class="mb-5">
      <input type="text" class="form-control" placeholder="Search">
    </div>
    <div class="mb-5">
      <h5 class="mb-4">Categories</h5>
      <div class="d-flex justify-content-between mb-3" v-for="item in categories" :key="item.id">
        <p class="mb-0">{{ item.name }}</p>
        <small>{{ item.total }}</small>
      </div>
    </div>

    <div>
      <h5 class="mb-4">Recent Posts</h5>
      <div class="d-flex gap-3 mb-4" v-for="post in recentPosts" :key="post.id">
        <img :src="post.image" width="80" class="rounded">
        <div>
          <p class="mb-1">{{ post.title }}</p>
          <small>{{ post.date }}</small>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const categories = [
  {
    id:1,
    name:"Crafts",
    total:2
  },
  {
    id:2,
    name:"Design",
    total:8
  },
  {
    id:3,
    name:"Handmade",
    total:7
  },
  {
    id:4,
    name:"Interior",
    total:1
  },
  {
    id:5,
    name:"Wood",
    total:6
  }
]

const recentPosts = [
  {
    id:1,
    image: "/svg/blogkanan1.svg",
    title: "Going all-in with millennial design",
    date: "03 Aug 2022"
  },
  {
    id:2,
    image: "/svg/blogkanan2.svg",
    title:"Exploring new ways of decorating",
    date:"03 Aug 2022"
  },
  {
    id:3,
    image: "/svg/bloghandmade.svg",
    title:"Handmade pieces that took time to make",
    date:"03 Aug 2022"
  },
  {
    id:4,
    image: "/svg/blogkanan4.svg",
    title:"Modern home in Milan",
    date:"03 Aug 2022"
  },
  {
    id:5,
    image:"/svg/blogkanan5.svg",
    title:"Colorful office redesign",
    date:"03 Aug 2022"
  }
]
</script>