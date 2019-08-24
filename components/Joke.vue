<template>
    <div id="joke">
        <button class="btn" v-on:click="getJoke">
        <h2 class="joke">{{ joke }}</h2>
        </button>
    </div>
</template>

<script>
import axios from "axios";

export default {
    data () {
        return {
            joke: null
        }
    },
    methods: {
        getJoke: function(event) {
            axios
                .get('https://icanhazdadjoke.com', {headers: {'Accept': 'text/plain'}})
                .then(response => (this.joke = response.data))
        }
    },
    created() {
        axios
            .get('https://icanhazdadjoke.com', {headers: {'Accept': 'text/plain'}})
            .then(response => (this.joke = response.data))
    }
}
</script>

<style scoped>
.joke {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  display: flex;
  align-items: center;
  text-align: center;
}
</style>