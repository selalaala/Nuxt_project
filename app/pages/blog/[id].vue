<template>
    <div>
        <Navbar />
        <PageBanner title="Blog Detail" />
        <Detailblog :blog="blog"/>
        <Quality />
        <Footer />
    </div>
</template>

<script setup>
import detailblog from '../../../data/detailblog.json'

const route = useRoute()
const blog = detailblog.find(
  item => item.id === Number(route.params.id)
)
</script>