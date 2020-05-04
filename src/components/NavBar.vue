<template>
  <div class="navbar">
    <div class="navbar__name">
      <router-link to="/" class="route">
        Lakshit Arora
      </router-link>
    </div>
    <ul class="navbar__ul">
      <router-link to="/" class="route">
        <i class="fas fa-home"></i>
        <li>Home</li>
      </router-link>
      <router-link to="/" class="route">
        <i class="fas fa-user"></i>
        <li>About</li>
      </router-link>
      <router-link to="/" class="route">
        <i class="fas fa-address-card"></i>
        <li>Resume</li>
      </router-link>
      <router-link to="/contact-me" class="route">
        <i class="fas fa-envelope"></i>
        <li>Contact</li>
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
    /*background-color: #091426;*/
    background-color: white;
  }

  .navbar {
    color: white;
    width: 100%;
    position: fixed;
    height: 38px;
    padding-top: 15px;

    &__name {
      float: left;
      padding-left: 20px;
      cursor: pointer;
    }
  }

  ul {
    display: flex;
    align-items: stretch;
    justify-content: space-between;
    width: 20%;
    margin: 0;
    float: right;
    padding: 0 20px 0 0;
    cursor: pointer;
  }

  li {
    display: block;
    flex: 0 1 auto;
    list-style-type: none;
  }

  i{
    i:hover{
      opacity: 0;
      transition-duration: 50ms;
    }
  }
</style>