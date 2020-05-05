<template>
  <div class="navbar">
    <div class="navbar__name">
      <router-link to="/" class="route">
        Lakshit Arora
      </router-link>
    </div>
    <ul class="navbar__ul">
      <router-link to="/" class="route">
        <i class="fas fa-home fa-lg"></i>
        <li>HOME</li>
      </router-link>
      <router-link to="/" class="route">
        <i class="fas fa-user fa-lg"></i>
        <li>ABOUT</li>
      </router-link>
      <router-link to="/" class="route">
        <i class="fas fa-address-card fa-lg"></i>
        <li>RESUME</li>
      </router-link>
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

  .navbar {
    color: #CCD6F6;
    width: 100%;
    position: fixed;
    height: 38px;
    padding-top: 20px;

    &__name {
      float: left;
      padding-left: 20px;
      cursor: pointer;
    }
  }
  a{
    color: #CCD6F6;
  }
  a:hover{
    color: #64FFDA;
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
  }
  i:hover{
    margin-top:-3px;
    padding:-1px;
    float:left;
    -webkit-transition: margin 100ms ease-out;
    -moz-transition: margin 100ms ease-out;
    -o-transition: margin 100ms ease-out;
    color: #64FFDA;
  }

</style>