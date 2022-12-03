<template>
    {{ cytat }}
</template>

<script>
import axios from 'axios'
export default {
    name: 'QuoteItem',
    data() {
        return {
            cytat: String
        }
    },
    methods: {
        async fetchData() {
            const daneResponse = await axios.get('https://api.chucknorris.io/jokes/random')
            this.cytat = daneResponse.data.value
            console.log(daneResponse.data.value)
        }
    },
    async mounted() {
        await this.fetchData()
    }
}
</script>