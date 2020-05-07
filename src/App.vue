<template>
  <div class="app">
    <nav-bar></nav-bar>
    <router-view/>
  </div>
</template>
<script>
  import NavBar from './components/NavBar'
  export  default {
    components:{
      NavBar,
    }
  }
</script>
<style>
  *{
    margin: 0px;
    background-color: #0a182f;
    font-family: "Montserrat";
  }
</style>
