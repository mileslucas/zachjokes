<template>
  <div>
    <Title />
    <div class="container-fluid">
      <Joke />

      <p id="click" class="pt-3">Click for more!</p>
    </div>
    <div class="footer fixed-bottom mx-auto">
      <p>
        <a href="/about" class="my-1">About</a> · Copyright © 2019
        <a href="https://mileslucas.com">Miles Lucas</a>
      </p>
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
@media (max-width: 375px) {
  #click {
    font-size: 10px;
  }
}
#click {
  color: #ffffff;
  text-align: center;
  font-size: 20px;
}
</style>

