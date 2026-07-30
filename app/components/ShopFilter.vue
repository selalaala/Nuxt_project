<template>
  <section class="shop-filter py-4">
    <div class="container">
      <div class="d-flex justify-content-between align-items-center">
        <div class="d-flex align-items-center gap-3">
            <i class="bi bi-sliders"></i>
            <p class="mb-0">Filter</p>
            <i class="bi bi-grid-fill"></i>
            <i class="bi bi-view-list"></i>
           <span>|</span>
            <p class="mb-0">Showing 1–16 of 32 results</p>
        </div>
        <div class="d-flex align-items-center gap-3">
          <label class="mb-0">Show</label>
          <input type="text" value="16" class="form-control w-auto">
          <label class="mb-0">Sort by</label>
          <input type="text" value="Default" class="form-control w-auto">
        </div>
      </div>
    </div>
  </section>
</template>

<style>
.shop-filter {
    background-color: #FFF3E3;
}
</style>