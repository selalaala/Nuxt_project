<template>
 <section class="furniture text-center">
    <p>Share your setup with</p>
    <h2>#FuniroFurniture</h2>
    <div class="gallery">
        <div class="left">
            <img src="../assets/svg/furniture-1.svg">
            <img src="../assets/svg/furniture-2.svg">
            <img src="../assets/svg/furniture-3.svg">
            <img src="../assets/svg/furniture-4.svg">
        </div>
        <div class="center">
            <img src="../assets/svg/furniture-5.svg">
        </div>
        <div class="right">
            <img src="../assets/svg/furniture-6.svg">
            <img src="../assets/svg/furniture-7.svg">
            <img src="../assets/svg/furniture-8.svg">
            <img src="../assets/svg/furniture-9.svg">
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
</style>