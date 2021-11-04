<template>
  <!-- Footer -->
<footer class="bg-grey text-center text-white">
  <!-- Grid container -->
  <div class="container p-4">

    <!-- Section: Text -->
    <section class="mb-4">
      <p>
        This web application shows that N00192514 can use the rest of Contries API and when clicking on countries you will be given a list of all the countries, you can also use the searchbar to find a specific country 
      </p>
    </section>
    <!-- Section: Text -->

    <!-- Section: Links -->
    <section class="">
      <!--Grid row-->
      <div class="row">
        <!--Grid column-->
        <div class="col-lg-3 col-md-6 mb-4 mb-md-0">
          <h5 class="text-uppercase">Useful Links</h5>

          <ul class="list-unstyled mb-0">
            <li>
              <router-link :to="{ name: 'countries' }">Countries</router-link>
            </li>
            <li>
              <router-link :to="{ name: 'about' }">About</router-link>
            </li>
            <li>
              <router-link :to="{ name: 'contact' }">Contact</router-link>
            </li>
          </ul>
        </div>
      </div>
        
      <!--Grid row-->
    </section>
    <!-- Section: Links -->
  </div>
  <!-- Grid container -->

  <!-- Copyright -->
  <div class="text-center p-3" style="background-color: rgba(0, 0, 0, 0.2);">
    © 2020 Copyright:
    <router-link :to="{ name: 'home' }">WorldVue.com</router-link>
  </div>
  <!-- Copyright -->
</footer>
<!-- Footer -->
</template>

<script>
export default {
  name: "Footer",
};
</script>

<style scoped>
* {
  background: #000000;
}
a:link, 
a:visited{
  color: rgb(255, 255, 255);
}
.text-reset{
  color: white !important;
}
.top {
  padding-top: 20px;
}
</style>