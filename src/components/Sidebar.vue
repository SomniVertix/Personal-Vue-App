<template>
  <div id="sidebar">
    <div v-bind:key="todo.id" v-for="todo in todos">
        <li>{{todo.title}}</li>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Sidebar',
  props:["todos"]
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
    #sidebar{
        background-color: lightblue;
        position: absolute;
        z-index: 10;
        top: 50%;
        left: 1rem;
        overflow-x: hidden;
        overflow-y: auto;
        -webkit-overflow-scrolling: touch;
        -ms-overflow-style: none;
    }

</style>
