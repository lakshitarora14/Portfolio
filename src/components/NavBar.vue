<template>
  <div class="navbar">
    <div class="navbar__name">
      <router-link to="/" class="route">
        <img src="../assets/image.png" class="navbar__logo" height="40px" width="40px">
        <div class="lakshit">LAKSHIT ARORA</div>
      </router-link>
    </div>
    <ul class="navbar__ul">
      <router-link to="/" class="route">
        <i class="fas fa-home fa-lg"></i>
        <li>HOME</li>
      </router-link>
      <router-link to="/about" class="route">
        <i class="fas fa-user fa-lg"></i>
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
    name: "NavBar.vue"
  }
</script>

<style scoped lang="scss">
  * {
    z-index: 1;
    background-color: #091426;
  }

  .lakshit {
    margin-left: 5px;
    display: inline;
    position: relative;
    bottom: 1vw;
    font-size: 18px;
  }

  .lakshit:hover {
    color: #64FFDA;
  }

  .navbar {
    color: #CCD6F6;
    width: 100%;
    position: fixed;
    height: 38px;
    padding-top: 20px;

    &__name {
      font-family: "PT Sans Narrow";
      float: left;
      cursor: pointer;
      position: absolute;
      top: 0.8vw;
      left: 1vw;
      display: inline;
    }
  }

  img {
    display: inline;
    background: transparent;
  }

  a {
    color: #CCD6F6;
    text-decoration: none;
  }

  ul {
    display: flex;
    align-items: stretch;
    justify-content: space-between;
    width: 22%;
    margin: 0;
    float: right;
    padding: 0 30px 0 0;
    cursor: pointer;
  }

  li {
    display: block;
    flex: 0 1 auto;
    list-style-type: none;
    visibility: hidden;
    font-family: "PT Sans Narrow";
  }

  i:hover {
    margin-top: -3px;
    padding: -2px;
    float: left;
    -webkit-transition: margin 100ms ease-out;
    -moz-transition: margin 100ms ease-out;
    -o-transition: margin 100ms ease-out;
    color: #64FFDA;
  }

</style>