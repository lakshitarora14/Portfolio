<template>
  <div class="app">
    <nav-bar></nav-bar>
    <router-view/>
  </div>
</template>
<script>
  import NavBar from './components/NavBar'

  export default {
    components: {
      NavBar,
    }
  }
</script>
<style lang="scss">
  $background: #0a182f;
  * {
    margin: 0px;
    background-color: $background;
    font-family: "Montserrat";
  }
</style>
