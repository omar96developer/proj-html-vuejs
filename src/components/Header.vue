<template>
  <header class="header_section ">
    <!-- NavBar w/info -->
    <!-- Info -->
    <nav class="nav_bar" id="id1">
      <div class="container-fluid nav_a">
        <div class="container-lg px-5">
          <div class="row">
            <div class="col-6 nav_a1 d-flex py-2">
              <p>We have a 95% Successful pass rate!</p>
            </div>
            <div class="col-6 nav_a2 d-flex justify-content-end py-2">
              <p><i class="fas fa-phone"></i> Give us a call to book your tuition! 1-800-555-555</p>
            </div>
          </div>
        </div>
      </div>
      <!-- logo and link -->
      <!-- dinamic -->
      <div class="container-fluid nav_b">
        <div class="container-lg px-5">
          <div class="row d-flex ">
            <div class="col-5 py-4 nav_b1">
              <img src="../assets/img/avada-drivers-logo-1x.png" alt="">
            </div>
            <div class="col-7 py-4 nav_b2 d-flex">
              <ul class="d-flex ">
                <Navbar v-for="(link, i) in navLink" :key="i" :links='link'></Navbar>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </nav>

    <!-- herotext -->
    <section>
      <div class="container-lg">
        <div class="row d-flex hero_section p-5">
          <div class="hero_section_a col-6 d-flex flex-column">
            <h1>Drive with Avada</h1>
            <p>We offer the finest driving tuition money can buy</p>
          </div>
         
        </div>
      </div>
    </section>
  <!-- icon -->
    <div class="hero_section_ico">
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
import Navbar from '@/components/Navbar.vue'


export default {
  name: 'Header',
  components: {
    Navbar
  },
  data() {
    return {
      navLink: [
        {
          link: '#id1',
          text: 'HOME'
        },
        {
          link: '#id2',
          text: 'ABOUT'
        },
        {
          link: '#id3',
          text: 'PRICES'
        },
        {
          link: '#id4',
          text: 'COURSES',
          newt: 'New'
        },
        {
          link: '#id5',
          text: 'LOCATION'
        },
        {
          link: '#id6',
          text: 'BLOG',
          
        },
        {
          link: 'id7',
          text: 'BOOK NOW',
          class: true,
        }
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
