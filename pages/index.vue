<template>
  <div>
    <Title />
    <div class="container-fluid">
      <Joke />
    </div>
    <div class="footer fixed-bottom mx-auto">
      <a href="/about" class="my-1">About</a>
      <p>Copyright © 2019 <a href="https://mileslucas.com">Miles Lucas</a></p>
    </div>
  </div>
</template>

<script>
import Title from "~/components/Title.vue";
import Joke from "~/components/Joke.vue";

export default {
  components: {
    Joke,
    Title
  }
};
</script>

<style>
.footer {
  margin-bottom: 1rem;
  color: #ffffffd2;
  width: 300px;
  text-align: center;
}
a {
  color: #e4e4e4;
}
</style>

