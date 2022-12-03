<template>
    <div :key="task.id" v-for="task in tasks">
        <p>{{ task.name }} {{ task.surname }}</p>
    </div>
</template>

<script>
export default {
    name: "ListItem",
    props: {
        tasks: Array
    }
}
</script>