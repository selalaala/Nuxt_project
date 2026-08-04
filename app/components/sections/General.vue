<template>
  <section class="compare-table py-5">
    <div class="container">
      <div class="row gx-4">
        <div class="col-lg-3 col-md-3 compare-col compare-title">
          <h3 class="section-title">General</h3>
          <div class="compare-item">Sales Package</div>
          <div class="compare-item">Model Number</div>
          <div class="compare-item">Secondary Material</div>
          <div class="compare-item">Configuration</div>
          <div class="compare-item">Upholstery Material</div>
          <div class="compare-item">Upholstery Color</div>

          <h3 class="section-title mt-5">Product</h3>
          <div class="compare-item">Filling Material</div>
          <div class="compare-item">Finish Type</div>
          <div class="compare-item">Adjustable Headrest</div>
          <div class="compare-item">Maximum Load Capacity</div>
          <div class="compare-item">Origin of Manufacture</div>

          <h3 class="section-title mt-5">Dimensions</h3>
          <div class="compare-item">Width</div>
          <div class="compare-item">Height</div>
          <div class="compare-item">Depth</div>
          <div class="compare-item">Weight</div>
          <div class="compare-item">Seat Height</div>
          <div class="compare-item">Leg Height</div>

          <h3 class="section-title mt-5">Warranty</h3>
          <div class="compare-item">Warranty Summary</div>
          <div class="compare-item">Warranty Service Type</div>
          <div class="compare-item">Covered in Warranty</div>
          <div class="compare-item">Not Covered in Warranty</div>
          <div class="compare-item">Domestic Warranty</div>
        </div>

        <div class="col-lg-3 col-md-3 compare-col">
          <div class="space-title"></div>
          <div class="compare-item">1 sectional sofa</div>
          <div class="compare-item">TFCBLIGRBL6SRHS</div>
          <div class="compare-item">Solid Wood</div>
          <div class="compare-item">L-shaped</div>
          <div class="compare-item">Fabric + Cotton</div>
          <div class="compare-item">Bright Grey & Lion</div>

          <div class="space-section"></div>
          <div class="compare-item">Foam</div>
          <div class="compare-item">Bright Grey & Lion</div>
          <div class="compare-item">No</div>
          <div class="compare-item">280 KG</div>
          <div class="compare-item">India</div>

          <div class="space-section"></div>
          <div class="compare-item">265.32 cm</div>
          <div class="compare-item">76 cm</div>
          <div class="compare-item">167.76 cm</div>
          <div class="compare-item">45 KG</div>
          <div class="compare-item">41.52 cm</div>
          <div class="compare-item">5.46 cm</div>

          <div class="space-section"></div>
          <div class="compare-item">1 Year Manufacturing Warranty</div>
          <div class="compare-item">
            For Warranty Claims or Any Product Related Issues Please Email at
            operations@trevifurniture.com
          </div>
          <div class="compare-item">
            Warranty Against Manufacturing Defect
          </div>
          <div class="compare-item">
            The Warranty Does Not Cover Damages Due To Usage Of The Product
            Beyond Its Intended Use And Wear & Tear In The Natural Course Of
            Product Usage.
          </div>
          <div class="compare-item">1 Year</div>
          <button class="btn btn-furniro mt-4">
            Add To Cart
          </button>
        </div>

        <div class="col-lg-3 col-md-3 compare-col">
          <div class="space-title"></div>
          <div class="compare-item">
            1 Three Seater, 2 Single Seater
          </div>
          <div class="compare-item">DTUBLIGRBL568</div>
          <div class="compare-item">Solid Wood</div>
          <div class="compare-item">L-shaped</div>
          <div class="compare-item">Fabric + Cotton</div>
          <div class="compare-item">Bright Grey & Lion</div>
          
          <div class="space-section"></div>
          <div class="compare-item">Matte</div>
          <div class="compare-item">Bright Grey & Lion</div>
          <div class="compare-item">Yes</div>
          <div class="compare-item">300 KG</div>
          <div class="compare-item">India</div>
        
          <div class="space-section"></div>
          <div class="compare-item">265.32 cm</div>
          <div class="compare-item">76 cm</div>
          <div class="compare-item">167.76 cm</div>
          <div class="compare-item">65 KG</div>
          <div class="compare-item">41.52 cm</div>
          <div class="compare-item">5.46 cm</div>

          <div class="space-section"></div>
          <div class="compare-item">
            1.2 Year Manufacturing Warranty
          </div>
          <div class="compare-item">
            For Warranty Claims or Any Product Related Issues Please Email at
            support@xyz.com
          </div>
          <div class="compare-item">
            Warranty of the product is limited to manufacturing defects only.
          </div>
          <div class="compare-item">
            The Warranty Does Not Cover Damages Due To Usage Of The Product
            Beyond Its Intended Use And Wear & Tear In The Natural Course Of
            Product Usage.
          </div>
          <div class="compare-item">3 Month</div>
          <button class="btn btn-furniro mt-4">
            Add To Cart
          </button>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.compare-col {
    border-right: 1px solid #e8e8e8;
    padding: 0 24px 40px;
}

.compare-col:last-child {
    border-right: none;
}

.section-title {
    font-size: 28px;
    font-weight: 600;
    margin-bottom: 30px;
}

.space-title {
    height: 72px;
}

.space-section {
    height: 86px;
}

.compare-item {
    min-height: 58px;
    display: flex;
    align-items: center;
    font-size: 16px;
    line-height: 1.7;
    border-bottom: 1px solid #e8e8e8;
    padding: 14px 0;
}

.compare-item:last-of-type {
    border-bottom: none;
}

@media (max-width: 1199px) {
  .compare-col {
    padding: 0 15px 30px;
  }

  .compare-item {
    font-size: 14px;
    line-height: 1.6;
    min-height: auto;
    padding: 12px 0;
    word-break: break-word;
  }

  .section-title {
    font-size: 24px;
  }
}
</style>