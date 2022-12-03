<template>
  <div class="home">
    <h1>Home page</h1>
    <ListItem :tasks="tasks" />
    <!-- {{ msg }} -->
    <!-- <ButtonItem msg="xd" /> -->
  </div>
</template>

<script>
import ListItem from "@/components/List.vue"
export default {
  name: 'HomeView',
  props: {
    tasks: Array
  },
  components: {
    ListItem
  }
}
</script>
