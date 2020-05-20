<template>
  <div class="app">
    <nav-bar class="desktop-navbar"></nav-bar>
    <mobile-navbar class="mobile-navbar"></mobile-navbar>
    <navbar-left></navbar-left>
    <navbar-right></navbar-right>
    <contact-me-navbar></contact-me-navbar>
    <router-view/>
  </div>
</template>
<script>
  import NavBar from './components/NavBar'
  import MobileNavbar from './components/MobileNavbar'
  import NavbarLeft from './components/NavbarLeft'
  import NavbarRight from './components/NavbarRight'
  import ContactMeNavbar from './components/ContactMeNavbar'
  export default {
    components: {
      ContactMeNavbar,
      NavbarRight,
      NavbarLeft,
      NavBar,
      MobileNavbar,
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
  @media screen and (max-width: 600px){
    .desktop-navbar{
      display: none;
    }
  }
  @media screen and (min-width: 601px){
    .mobile-navbar{
      display: none;
    }}
</style>
