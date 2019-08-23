<template>
  <section class="container">
    <div>
      <h1 class="title">Zach Jokes</h1>
      <app-logo />
      <joke />
    </div>
  </section>
</template>

<script>
import AppLogo from "~/components/AppLogo.vue";
import Joke from "~/components/Joke.vue";

export default {
  components: {
    AppLogo,
    Joke
  },
};
</script>

<style>
.container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}

.title {
  font-family: "Quicksand", "Source Sans Pro", -apple-system, BlinkMacSystemFont,
    "Segoe UI", Roboto, "Helvetica Neue", Arial, sans-serif; /* 1 */
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  max-width: 70%;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
  display: block;
  margin-left: auto;
  margin-right: auto;
}

.links {
  padding-top: 15px;
}
</style>

