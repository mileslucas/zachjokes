<template>
    <div id="joke">
        <button v-on:click="getJoke">Moar!!</button>
        <h2 class="subtitle">{{ joke }}</h2>
    </div>
</template>

<script>
import axios from "axios";

function getJoke() {
    return ;
}

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