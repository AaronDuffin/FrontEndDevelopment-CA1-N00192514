<template>
  <div>
    <b-container-fluid>
          <NavBar />
              <router-view />
          <Footer/>
    </b-container-fluid>
  </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";
import Footer from './components/Footer.vue';

export default {
  name: "App",
  components: {
    NavBar,
    Footer,
  },
};
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Lato:ital,wght@0,100;0,300;1,100;1,300&display=swap');
#app {
  font-family: 'Lato', sans-serif;
}
*{
    background-color: #424C55;
}

</style>
