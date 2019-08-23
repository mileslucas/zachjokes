<template>
    <h2 class="subtitle">{{ joke }}</h2>
</template>

<script>
import axios from "axios";

export default {
    data () {
        return {
            joke: null
        }
    },
    mounted() {
        axios
            .get('https://icanhazdadjoke.com', {'headers': {'Accept': 'text/plain'}})
            .then(response => (this.joke = response.data))
    }
}
</script>