<template>
  <footer>
    <section class="footer_a text-white">
      <div class="container-lg d-flex p-5">
        <div class="row">

          <div class="col-3 d-flex flex-column">
            <img src="../assets/img/avada-drivers-logo-1x.png" alt="logo">
            <p class="mt-3">Avada Driving School is the right choise for experianced drivers looking for a refresher course, or the brand new drive wanting to pass first time.</p>
          </div>

          <div class="col-6 d-flex justify-content-around">
            <div>
              <h5 class="mb-4">CONTACT DETAILS</h5>
              <ul class="p-0">
                <ListA v-for="(contact, i) in contacts" :key="i" :contact='contact'></ListA>

                <!-- <li><i class="fas fa-home fs-5"></i><span class="ms-3">12345 North main Street.</span></li>
                <li><i class="fas fa-phone fs-5"></i><span class="ms-3">NewYork. NY 555555</span></li>
                <li><i class="fas fa-phone fs-5"></i><span class="ms-3">1.800.555.6789</span> </li> 
                <li><i class="fas fa-envelope fs-5"></i> <span class="ms-3">info@your-domain.com </span></li>
                <li><i class="fas fa-link fs-5"></i> <span class="ms-3">Theme-Fusion.com </span></li> -->
              </ul>
            </div>
            <div>
              <h5 class="mb-4">COURSES</h5>
              <ul class="p-0">
               <ListB v-for="(corse, i) in courses" :key="i" :corse='corse'></ListB>
               
                <!-- <li><i class="far fa-arrow-alt-circle-right fs-5 me-3"></i> Pass Plus</li>
                <li><i class="far fa-arrow-alt-circle-right fs-5 me-3"></i> Intensive Course</li>
                <li><i class="far fa-arrow-alt-circle-right fs-5 me-3"></i> Automatic</li>
                <li><i class="far fa-arrow-alt-circle-right fs-5 me-3"></i> Instructor Training</li> -->
              </ul>  
            </div>         
          </div>
          
          <div class="col-3 text-center">
            <img src="../assets/img/avada-drivers-logo-1x.png" alt="#">
            <button type="button" class="btn  mt-5">BOOK NOW</button>
          </div>
        </div>      
      </div>
    </section>
    <section class="footer_b">
      <div class="container-lg">
        <div class="row px-5 py-4 text-white">
          <div class="col-8">
            <p><i class="far fa-copyright"></i> Copyright 2012 - 2020: Avada Theme by <span>ThemeFusion</span>  | All Right Reserved | Powered by <span>WordPress</span> </p>
          </div>
          <div class="col-4 text-end">
            <span><i class="fab fa-facebook-f me-3"></i><i class="fab fa-twitter me-3"></i><i class="fab fa-youtube me-3"></i><i class="fab fa-instagram"></i></span>
          </div>
        </div>
      </div>
    </section>
  </footer>
</template>

<script>
import ListA from '@/components/ListA.vue'
import ListB from '@/components/ListB.vue'


export default {
  name: 'Footer',
  components: {
    ListA,
    ListB
    
  },
  data(){
    return {
      contacts: [    
        {
          class: 'fas fa-home fs-5',
          text: '12345 North main Street. NewYork. NY 555555'
        },
         {
          class: 'fas fa-phone fs-5',
          text: '1.800.555.6789'
        },
         {
          class: 'fas fa-envelope fs-5',
          text: 'info@your-domain.com '
        },
         {
          class: 'fas fa-link fs-5',
          text: 'Theme-Fusion.com '
        }
      ],
      courses: [
        {
          class: 'far fa-arrow-alt-circle-right fs-5 me-3',
          text: 'Pass Plus'
        },
        {
          class: 'far fa-arrow-alt-circle-right fs-5 me-3',
          text: 'Intensive Course'
        },
        {
          class: 'far fa-arrow-alt-circle-right fs-5 me-3',
          text: 'Automatic'
        },
        {
          class: 'far fa-arrow-alt-circle-right fs-5 me-3',
          text: 'Instructor Training'
        },
      ]
    }
  }
}
</script>

<style lang="scss">

</style>
