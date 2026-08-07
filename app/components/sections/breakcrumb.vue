<template>
    <section class="breadcrumb py-3">
        <div class="container">
            <p class="text-secondary m-3">Home > Shop >
                <span class="mx-3">|</span>
                <span class="text-black ms-2">{{ title }}</span>
            </p> 
        </div>
    </section>
</template>

<style scoped>
.breadcrumb {
    background-color: #FFF3E3;
}
</style>

<script setup>
defineProps({
  title: {
    type: String,
    required: true
  }
})
</script>