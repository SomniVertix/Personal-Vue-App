<template>
  <div id="hello">
    <h1>{{ msg }}</h1>
    <div id="right-container-div">
      <a href="google.com" class="inner-right-containers"> HOME </a>
      <a href="google.com" class="inner-right-containers"> PROJECTS </a>
      <a href="google.com" class="inner-right-containers"> *NEW* UPCOMING </a>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Header',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
  #hello {
    display: grid;
    width: 100%;
    height: 3.5rem;
    background-color: #36454f;
    grid-template-columns: 3fr 1fr;
  }

  h1{
    margin: 0;
    color: white;
  }

  #right-container-div {
    display: flex;
    justify-content: space-around;
  }

  .inner-right-containers {
    color: white;
    text-decoration: none;
    padding: 1rem;
    text-align: center;
    vertical-align: middle;
  }

</style>
