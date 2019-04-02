<template>
  <div id="app">
    <Header msg="SOMNI.DEV"/>
    <Sidebar v-bind:todos="todos"/>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import Sidebar from './components/Sidebar.vue'

export default {
  name: 'app',
  components: {
    Header,
    Sidebar
  },
  data() {
    return {
      todos: [
        {
          id: 1,
          title: "Who?"
        },
        {
          id: 2,
          title: "What?"
        },
        {
          id: 3,
          title: "How?"
        }
      ]
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin: 0px;
}

body {
  margin: 0;
}
</style>
