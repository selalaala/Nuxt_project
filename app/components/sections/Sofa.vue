<template>
  <section class="py-3">
    <div class="container">
      <div class="row g-5">
        <div class="col-lg-6">
          <div class="row">
            <div class="col-2">
              <div class="d-flex flex-column gap-3">
                <div>
                  <img src="/svg/sofa.svg" class="img-fluid">
                </div>
                <div>
                  <img src="/svg/sofa.svg" class="img-fluid">
                </div>
                <div>
                  <img src="/svg/sofa.svg" class="img-fluid">
                </div>
                <div>
                  <img src="/svg/sofa.svg" class="img-fluid">
                </div>
              </div>
            </div>

            <div class="col-10">
              <div class="text-center">
                <img src="/svg/sofa.svg" class="img-fluid">
              </div>
            </div>
          </div>
        </div>
        
        <div class="col-lg-6">
          <h1 class="fw-normal mb-2">
            Asgaard sofa
          </h1>
          <h4 class="text-secondary mb-3">
            Rs. 250,000.00
          </h4>
          <div class="d-flex align-items-center gap-3 mb-3">
            <div class="text-warning">
              <i class="bi bi-star-fill"></i>
              <i class="bi bi-star-fill"></i>
              <i class="bi bi-star-fill"></i>
              <i class="bi bi-star-fill"></i>
              <i class="bi bi-star-half"></i>
            </div>
            <div class="vr"></div>
            <small class="text-secondary">
              5 Customer Review
            </small>
          </div>
          <p class="text-secondary">
            Setting the bar as one of the loudest speakers in its class...
          </p>
          <small class="text-secondary">
            Size
          </small>
          <div class="d-flex gap-2 mt-2 mb-4">
            <button class="btn btn-furniro btn-sm">
              L
            </button>
            <button class="btn btn-light btn-sm border">
              XL
            </button>
            <button class="btn btn-light btn-sm border">
              XS
            </button>
          </div>
          <small class="text-secondary">
            Color
          </small>
          <div class="d-flex gap-3 mt-2 mb-4">
            <span class="rounded-circle bg-primary color-dot"></span>
            <span class="rounded-circle bg-dark color-dot"></span>
            <span class="rounded-circle bg-furniro color-dot"></span>
          </div>

          <div class="d-flex flex-wrap gap-3">
            <div class="border rounded d-flex align-items-center px-3 py-2">
              <button class="btn btn-sm">-</button>
              <span class="mx-3">1</span>
              <button class="btn btn-sm">+</button>
            </div>
            <NuxtLink to="/cart" class="btn btn-outline-dark px-4 py-3">Add To Cart</NuxtLink>
            <NuxtLink to="/produk-comparison" class="btn btn-outline-dark px-4 py-3">+ Compare</NuxtLink>
          </div>

          <hr class="my-5">
          <table class="table table-borderless text-secondary">
            <tbody>
              <tr>
                <td width="120">SKU</td>
                <td>: SS001</td>
              </tr>
              <tr>
                <td>Category</td>
                <td>: Sofas</td>
              </tr>
              <tr>
                <td>Tags</td>
                <td>: Sofa, Chair, Home, Shop</td>
              </tr>
              <tr>
                <td>Share</td>
                <td>
                  <i class="bi bi-facebook me-3"></i>
                  <i class="bi bi-linkedin me-3"></i>
                  <i class="bi bi-twitter-x"></i>
                </td>
              </tr>
            </tbody>
          </table>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.btn-default {
    border-color: black;
}

.bg-furniro{
    background:#B88E2F;
}

.color-dot{
    width:30px;
    height:30px;
    display:inline-block;
}

@media (max-width: 991px){
    section{
        padding-top: 10px !important;
    }
}
</style>
