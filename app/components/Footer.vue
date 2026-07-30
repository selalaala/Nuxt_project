<template>
  <footer class="py-5">
    <div class="container">
      <div class="row">
        <div class="col-lg-4">
          <h3>Furniro.</h3>
          <p>400 University Drive Suite 200 Coral<br> Gables, <br>FL 33134 USA</p>
        </div>
        <div class="col-lg-2">
          <h6>Links</h6>
          <ul class="list-unstyled">
            <li><NuxtLink to="/">Home</NuxtLink></li>
            <li><NuxtLink to="/shop">Shop</NuxtLink></li>
            <li><NuxtLink to="/blog">Blog</NuxtLink></li>
            <li><NuxtLink to="/contact">Contact</NuxtLink></li>
          </ul>
        </div>
        <div class="col-lg-2">
          <h6>Help</h6>
          <ul class="list-unstyled">
            <li><a href="#">Payment Options</a></li>
            <li><a href="#">Returns</a></li>
            <li><a href="#">Privacy Policies</a></li>
          </ul>
        </div>
        <div class="col-lg-4">
          <h6>Newsletter</h6>
          <div class="d-flex">
            <input class="form-control" placeholder="Enter Your Email Address">
            <button class="btn btn-link text-black">SUBSCRIBE</button>
          </div>
        </div>
      </div>
    </div>
</footer>
</template>

<style>
footer ul{
    padding: 0;
}

footer li{
    list-style: none;
    margin-bottom: 15px;
}

footer a{
    text-decoration: none;
    color: #000;
    transition: 0.3s;
}

footer a:hover{
    color: #B88E2F;
}
</style>