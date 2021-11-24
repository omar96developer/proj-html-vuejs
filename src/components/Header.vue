<template>
  <header class="header_section ">
    <!-- NavBar w/info -->
    <!-- Info -->
    <nav class="nav_bar">
      <div class="container-fluid nav_a">
        <div class="container-lg border px-5">
          <div class="row">
            <div class="col-6 nav_a1 border d-flex py-2">
              <p>We have a 95% Successful pass rate!</p>
            </div>
            <div class="col-6 nav_a2 border d-flex justify-content-end py-2">
              <p><i class="fas fa-phone"></i> Give us a call to book your tuition! 1-800-555-555</p>
            </div>
          </div>
        </div>
      </div>
      <!-- logo and link -->
      <!-- dinamic -->
      <div class="container-fluid nav_b">
        <div class="container-lg border px-5">
          <div class="row d-flex ">
            <div class="col-5 py-4 nav_b1 border">
              <img src="../assets/img/avada-drivers-logo-1x.png" alt="">
            </div>
            <div class="col-7 py-4 nav_b2 border d-flex">
              <ul class="d-flex ">
                <li><a href="">HOME</a></li>
                <li><a href="">ABOUT</a></li>
                <li><a href="">PRICES</a></li>
                <li><a href="">COURSES</a></li>
                <li><a href="">LOCATIONS</a></li>
                <li><a href="">BLOG</a></li>
                <li><a class="nav-btn" href="#">BOOK NOW</a></li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <!-- herotext -->
    <section>
      <div class="container-lg border">
        <div class="row d-flex hero_section p-5">
          <div class="hero_section_a col-6 border d-flex flex-column">
            <h1>Drive with Avada</h1>
            <p>We offer the finest driving tuition money can buy</p>
          </div>
         
        </div>
      </div>
    </section>
  <!-- icon -->
    <div class="hero_section_ico border">
        <div class="hero_ico_1 mb-2 d-flex flex-column">
          <i class="fab fa-gripfire fs-2"></i>
          <p class="fs-6 text-black m-0">Demos</p>
        </div>
        <div class="hero_ico_2 d-flex flex-column">
          <p class="m-0 fw-bold"><span class="">$</span><span class="fs-2 align-middle">39</span></p>
          <p class="text-black fs-6">On Sale</p>
        </div>
    </div>
  </header>
</template>


<script>

export default {
  name: 'Header',
  components: {
  }
}
</script>

<style lang="scss">

</style>
