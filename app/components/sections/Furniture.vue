<template>
 <section class="furniture text-center">
    <p>Share your setup with</p>
    <h2>#FuniroFurniture</h2>
    <div class="gallery">
        <div class="left">
            <img v-for="item in leftImages" :key="item.id" :src="item.image">
        </div>
        <div class="center">
            <img :src="centerImage.image">
        </div>
        <div class="right">
            <img v-for="item in rightImages" :key="item.id":src="item.image">
        </div>
    </div>
 </section>
</template>

<style>
.furniture {
    padding: 50px 50px;
}

.gallery{
    display: grid;
    grid-template-columns: 1fr 1.2fr 1fr;
    gap: 16px;
    padding: 20px;
    align-items: center;
}

.left,
.right{
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    gap: 16px;
}

.center img{
    width: 100%;
    height: 600px;
    object-fit: cover;
}

.left img,
.right img{
    width: 100%;
    height: 220px;
    object-fit: cover;
}

@media (max-width: 768px) {
    .gallery{
        grid-template-columns: 1fr;
    }

    .left,
    .right{
        grid-template-columns: 1fr;
    }

    .center img,
    .left img,
    .right img{
        width: 100%;
        height: auto;
    }
}
</style>
<script setup>
import { computed } from 'vue'
const props = defineProps({
  furnitures: Array
})
const leftImages = computed(() =>
  props.furnitures.filter(item => item.position === 'left')
)
const centerImage = computed(() =>
  props.furnitures.find(item => item.position === 'center')
)
const rightImages = computed(() =>
  props.furnitures.filter(item => item.position === 'right')
)
</script>