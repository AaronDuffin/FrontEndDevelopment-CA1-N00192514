<template>
  <div>
    <b-button v-b-toggle.sidebar-no-header>WorldVue</b-button>
    <b-sidebar id="sidebar-no-header" aria-labelledby="sidebar-no-header-title" no-header>
      <template #default="{ hide }">
        <div class="p-3">
          <nav class="mb-3">
            <b-nav vertical>
              <b-nav-item active @click="hide"><router-link :to="{ name: 'home' }">WorldVue</router-link></b-nav-item>
              <b-nav-item href="#link-1" @click="hide"><router-link :to="{ name: 'countries' }">Countries</router-link></b-nav-item>
              <b-nav-item href="#link-2" @click="hide"><router-link :to="{ name: 'about' }">About</router-link></b-nav-item>
              <b-nav-item href="#link-3" @click="hide"><router-link :to="{ name: 'contact' }">Contact</router-link></b-nav-item>
            </b-nav>
          </nav>
          <b-button variant="secondary" block @click="hide">Close Sidebar</b-button>
        </div>
      </template>
    </b-sidebar>
  </div>
</template>

<script>
export default {
  name: "NavBar",
};
</script>

<style scoped>
* {
  background: #424C55;
}

.navbar {
  padding: 10px;
  background: #424C55;
  text-decoration-line: none;
}

.h1 {
  font-size: 36px;
}

.h4{
  color: #ffffff !important;
}
.links {
  align-content: flex-end;
}

.sidebar-no-header-title{
  color: #ffffff !important; 
}
ul.nav li a,
ul.nav li a:visited {
  color: rgb(255, 255, 255) !important;
      text-decoration-line: none;

}

ul.nav li a:hover,
ul.nav li a:active {
  color: #000000 !important;
      text-decoration-line: none;

}

ul.nav li.active a {
  color: #000000 !important;
      text-decoration-line: none;

}
</style>