<template>
  <div class="navbar">
    <div class="navbar__name">
      <img src="../assets/image.png" class="navbar__logo" height="40px" width="40px">
      <router-link to="/home" class="route">
        <div class="lakshit">LAKSHIT ARORA</div>
      </router-link>
    </div>
    <ul class="navbar__ul">
      <router-link to="/home" class="route">
        <li>HOME</li>
      </router-link>
      <router-link to="/about" class="route">
        <li>ABOUT</li>
      </router-link>
      <a href="https://drive.google.com/open?id=1IZNCMK7dCITffbrvi9_s8_6yIUXx4OK7" target="_blank">
        <i class="fas fa-address-card fa-lg"></i>
        <li>RESUME</li>
      </a>
      <router-link to="/contact-me" class="route">
        <i class="fas fa-envelope fa-lg"></i>
        <li>CONTACT</li>
      </router-link>
    </ul>
  </div>
</template>

<script>
  export default {
    name: "MobileNavbar"
  }
</script>

<style scoped>

</style>