<template>
  <div class="container py-5">
    <div class="row g-5">
      <div class="col-lg-7">
        <h2 class="fw-bold mb-4">Billing details</h2>
        <form>
          <div class="d-flex gap-3 mb-0 w-75">
            <div class="col-md-6 mb-3">
              <label class="form-label">First Name</label>
              <input type="text" class="form-control">
            </div>
            <div class="col-md-6 mb-3">
              <label class="form-label">Last Name</label>
              <input type="text" class="form-control">
            </div>
          </div>
          <div class="mb-3">
            <label class="form-label">Company Name (Optional)</label>
            <input type="text" class="form-control">
          </div>
          <div class="mb-3">
            <label class="form-label">Country / Region</label>
            <select class="form-select">
                <option>Sri Lanka</option>
            </select>
          </div>
          <div class="mb-3">
            <label class="form-label">Street Address</label>
            <input type="text" class="form-control">
          </div>
          <div class="mb-3">
            <label class="form-label">Town / City</label>
            <input type="text" class="form-control">
          </div>
          <div class="mb-3">
            <label class="form-label">Province</label>
            <select class="form-select">
              <option>Western Province</option>
            </select>
          </div>
          <div class="mb-3">
            <label class="form-label">ZIP Code</label>
            <input type="text" class="form-control">
          </div>
          <div class="mb-3">
            <label class="form-label">Phone</label>
            <input type="text" class="form-control">
          </div>
          <div class="mb-3">
            <label class="form-label">Email Address</label>
            <input type="email" class="form-control">
          </div>
          <div class="mb-3">
            <textarea class="form-control" rows="4" placeholder="Additional Information"></textarea>
          </div>
        </form>
      </div>
      
      <div class="col-lg-5">
        <h5 class="fw-bold mb-4">Product</h5>
        <div class="d-flex justify-content-between mb-3">
            <span>Asgaard sofa × 1</span>
            <span>Rs. 250,000.00</span>
        </div>
        <div class="d-flex justify-content-between mb-3">
            <span>Subtotal</span>
            <span>Rs. 250,000.00</span>
        </div>
        <div class="d-flex justify-content-between border-bottom pb-3 mb-3">
            <strong>Total</strong>
            <strong class="text-warning">Rs. 250,000.00</strong>
        </div>
        <div class="form-check">
            <input class="form-check-input" type="radio" checked>
            <label class="form-check-label">Direct Bank Transfer</label>
        </div>
        <p class="small text-muted my-3">Make your payment directly into our bank account. Please use your Order ID as the payment reference. Your order will not be shipped until the funds have cleared in our account.</p>
        <div class="form-check mb-4">
            <input class="form-check-input" type="radio">
            <label class="form-check-label">Direct Bank Transfer</label>
        </div>
        <div class="form-check mb-4">
            <input class="form-check-input" type="radio">
            <label class="form-check-label">Cash On Delivery</label>
        </div>
        <p class="small text-muted my-3">Your personal data will be used to support your experience throughout this website, to manage access to your account, and for other purposes described in our privacy policy.</p>
        <div class="text-center">
            <button class="btn btn-outline-dark px-5">Place order</button>
        </div>
    </div>
</div>
</div>
</template>

<style scoped>
.form-control,
.form-select{
    height: 60px;
    border-radius: 10px;
    border: 1px solid #d9d9d9;
}

textarea.form-control{
    height: 120px;
    resize: none;
}

</style>