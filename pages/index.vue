<template>
<div>
  <header class="d-flex justify-content-center">
    <h1 class="title">Zach Jokes</h1>
  </header>
  <div class="container-fluid">
    <joke />
  </div>
  <footer class="fixed-bottom d-flex justify-content-center">
    Copyright © 2019 Miles Lucas
  </footer>
</div>
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";
import Joke from "~/components/Joke.vue";

export default {
  components: {
    AppLogo,
    Joke
  }
};
</script>

<style>

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

footer {
  padding-bottom: 1rem;
}

</style>

