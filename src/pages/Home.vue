<template>
  <div>
    <div>
      <b-container>
        <h1 class="hero">
            Welcome to WorldVue, You're number one stop to view all the countries of the world for youre next hoilday
            <br>
          <div center class="Video">
            <section>
              <iframe width="1100" height="500" src="https://www.youtube.com/embed/5pOFKmk7ytU?start=20" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
            </section>
          </div>
            <br>
            To see all the information about you're next destination please click the countries link to get started
          </h1>
          <br/>
        <br/>
        
        <br />
        <b-row>
          <b-img
            center
            src="https://cdn01.buxtonco.com/news/2661/istock-665028882__large.jpg"
            fluid
            alt="Responsive image">
          </b-img>
          <br />
        </b-row>
        <br/>
        <br/>
      </b-container>
    </div>
  </div>
</template>

<script>

export default {
  name: "home",
  components: {
  },
};
</script>



<style scoped>
* {
  background: #ffffff;
}
.hero {
  padding-top: 20px;
  text-align: center;
  color: #050505;
  font-weight: lighter;
  letter-spacing: 1px;
}
.searchtext{
  color: #000000;
  font-size: 18px;
}

</style>