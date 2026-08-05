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
                    <BlogKanan :categories="categories" :recentPosts="recentPosts" />
                </div>
            </div>
        </div>
        <Quality />
        <Footer />
  </div>
</template>


<script setup>
import blogs from '../../data/blog.json'
import categories from '../../data/categories.json'
import recentPosts from '../../data/recentPosts.json'
</script>