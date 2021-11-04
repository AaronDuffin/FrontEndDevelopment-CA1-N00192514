<template>
  <div class="background">
    <h1 class="title">All Countries</h1>
    <div class="search-box center">
      <input type="text" v-model="term" v-on:keyup.enter="searchCountries()" />
      <br>
      <br>
      <b-button
        class="float-end"
        variant="secondary"
        @click="searchCountries()"
        >Search</b-button>
    </div>
    <br>
      <b-card-group>
        <b-card>
            <CountryViewer
              v-for="country in countries"
              :key="country.ccn3"
              :country="country"
            />
        </b-card>
      </b-card-group>
  </div>
</template>

<script>
import axios from "axios";
import CountryViewer from "@/components/CountryViewer";

export default {
  name: "AllCountries",
  components: {
    CountryViewer,
  },
  data() {
    return {
      countries: [],
    };
  },
  mounted() {
    axios
      .get("https://restcountries.com/v3.1/all")
      .then((response) => {
        console.log(response.data);
        this.countries = response.data;
      })
      .catch((error) => console.log(error));
  },
  methods: {
    searchCountries() {
      if (!this.term) {
        alert("Please enter a country name");
        this.$byToast.toast("Please enter a country name", {
          title: "Warning",
          variant: "danger",
          toaster: "b-toaster-top-center",
          autoHideDelay: 6900,
          solid: true,
        });
        return;
      }
      axios
        .get(`https://restcountries.com/v3.1//name/${this.term}`)
        .then((response) => {
          console.log(response.data);
          this.countries = response.data;
        })
        .catch((error) => console.log(error));
    },
  },
};
</script>

<style>
* {
  background: #ffffff;
}
.title {
  text-align: center;
  color: #000000;
}
.b-button {
  color: aliceblue;
}

</style>
