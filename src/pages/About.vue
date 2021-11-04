<template>
  <div class="about">
    <b-container>
      <b-row>
        <b-col class="blacktext">
          <h1>This is the About Page</h1>
          <h4>
            This assignment is to show my ability to use a router.js to trasnsition through pages without using a href and to also how how i displayed all Countries of the world using a API
          </h4>
          <b-img
            center
            src="https://pbs.twimg.com/media/CCNxWJdUAAEo7Pq.png"
            fluid
            alt="Responsive image"
          >
          </b-img>
        </b-col>
      </b-row>
    </b-container>
  </div>
</template>

<script>

export default {
  name: "about",
};
</script>

<style scoped>
.blacktext {
  color: #000000;
}
</style>