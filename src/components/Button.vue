<template>
    <button @click="onClick()">{{ msg }}</button>
</template>

<script>
export default {
    name: "ButtonItem",
    props: {
        msg: String
    },
    methods: {
        onClick() {
            console.log("clicked")
        }
    }
}
</script>