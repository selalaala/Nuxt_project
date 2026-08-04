<template>
    <section class="quality">
        <div class="container pb-5">
            <div class="row">
                <div class="col-lg-3 col-md-6 mb-4">
                    <div class="d-flex align-items-center">
                        <img src="/svg/quality.svg" width="60" alt="">
                        <div class="ms-3">
                            <h5>High Quality</h5>
                            <p class="mb-0">crafted from top materials</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 mb-4">
                    <div class="d-flex align-items-center">
                        <img src="/svg/guarante.svg" width="60" alt="">
                        <div class="ms-3">
                            <h5>Warranty Protection</h5>
                            <p class="mb-0">Over 2 years</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 mb-4">
                    <div class="d-flex align-items-center">
                        <img src="/svg/shipping.svg" width="60" alt="">
                        <div class="ms-3">
                            <h5>Free Shipping</h5>
                            <p class="mb-0">Order over 150 $</p>
                        </div>
                    </div>
                </div>
                <div class="col-lg-3 col-md-6 mb-4">
                    <div class="d-flex align-items-center">
                        <img src="/svg/support.svg" width="60" alt="">
                        <div class="ms-3">
                            <h5>24 / 7 Support</h5>
                            <p class="mb-0">Dedicated support</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style>
.quality {
    background: #FCF8F3;
}

@media (max-width: 767px){
    .quality .col-md-6{
        display: flex;
        justify-content: center;
        margin-bottom: 20px;
    }

    .quality .d-flex{
        width: 260px;
    }
}
</style>