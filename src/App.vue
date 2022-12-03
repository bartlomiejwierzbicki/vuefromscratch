<template>
  <nav>
    <router-link class="link" to="/" msg="asd">Home</router-link> |
    <router-link class="link" to="/about">About</router-link>
  </nav>
  <div class="content"><router-view :tasks="tasks" /></div>
</template>

<script>

export default {
  name: 'App',
  data() {
    return { tasks: [] }
  },
  created() {
    this.tasks = [
      {
        id: 1,
        name: 'Chuck',
        surname: 'Norris',
        date: '02.01.1956'
      },
      {
        id: 2,
        name: 'Barack',
        surname: 'Obama',
        date: '01.05.1969'
      },
      {
        id: 3,
        name: 'Harry',
        surname: 'Potter',
        date: '01.01.1987'
      }

    ]
  }
}

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
}

nav {
  padding: 0px;
}

.link {
  text-decoration: none;
}

nav a {
  font-weight: bold;
  color: #2c3e50;
}

nav a.router-link-exact-active {
  color: #0188f7;
}
</style>
