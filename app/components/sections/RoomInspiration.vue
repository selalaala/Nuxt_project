<template>
<section class="room-section py-5">
    <div class="container">
        <div class="row align-items-center gy-4">
            <div class="col-lg-4">
                <h2 class="fw-bold display-6">50+ Beautiful rooms inspiration</h2>
                <p class="text-secondary my-4">Our designer already made a lot of beautiful prototype of rooms that inspire you.</p>
                <button class="btn btn-room px-4 py-3"> <NuxtLink to="/shop" class="text-white text-decoration-none">Explore More</NuxtLink></button>
            </div>
            <div class="col-lg-4">
                <div class="position-relative">
                    <img src="/svg/inner-peace.svg" class="img-fluid w-100 room-img" alt="">
                    <div class="room-info position-absolute">
                            <small class="text-secondary"> 01 —— Bed Room</small>
                            <h4 class="fw-bold mt-2">Inner Peace</h4>
                    </div>
                    <button class="btn btn-room position-absolute room-arrow"> →</button>
                </div>
            </div>
            <div class="col-lg-4">
                <img src="/svg/kitchen.svg" class="img-fluid w-100 room-img" alt="">
                <div class="d-flex justify-content-center gap-2 mt-4">
                    <span class="dot active"></span>
                    <span class="dot"></span>
                    <span class="dot"></span>
                    <span class="dot"></span>
                </div>
            </div>
        </div>
    </div>
</section>
</template>

<style>
.room-section{
    background: #FCF8F3;
}

.room-img{
    height:580px;
    object-fit:cover;
}

.btn-room{
    background: #B88E2F;
    color: #fff;
    border:none;
}

.btn-room:hover{
    background: #a67d25;
    color: #fff;
}

.dot{
    width:12px;
    height:12px;
    border-radius:50%;
    background:#D8D8D8;
}

.active{
    background: #B88E2F;
}
.room-info{
    background: #FCF8F3;
    padding: 20px;
    bottom: 24px;
    left: 24px;
    width: 220px;
}

.room-arrow{
    bottom: 24px;
    left: 244px;
    width: 48px;
    height: 48px;
    border-radius: 0;
}
</style>
