<template>
  <div class="navbar">
    <div class="navbar__name">
      <img src="../assets/image.png" class="navbar__logo" height="35px" width="35px">
      <router-link to="/home" class="route">
        <div class="lakshit">LAKSHIT ARORA</div>
      </router-link>
    </div>
    <div class="navbar__buttons">
      <router-link to="/home" class="route">
        <i class="fas fa-home fa-lg"></i>
      </router-link>
      <router-link to="/about" class="route">
        <i class="fas fa-user fa-lg"></i>
      </router-link>
      <a href="https://drive.google.com/file/d/1x16Pf2L04EQl7R9oIc8L7toeapkJeCjc/view?usp=sharing" target="_blank">
        <i class="fas fa-address-card fa-lg"></i>
      </a>
      <router-link to="/contact-me" class="route">
        <i class="fas fa-envelope fa-lg"></i>
      </router-link>
    </div>
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
    color: #CCD6F6;
    margin-left: 5px;
    display: inline-flex;
    position: relative;
    bottom: 1vw;
    font-size: 18px;
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-image: linear-gradient(
            0deg,
            #64FFDA,
            #64FFDA 50%,
            #CCD6F6 10%);
    background-size: 100% 200%;
    background-position: 0% 0%;
  }

  .lakshit:hover {
    transition: all 1s cubic-bezier(0.000, 0.000, 0.230, 1);
    background-position: 100% 100%;
  }

  .navbar {
    color: #CCD6F6;
    width: 100%;
    position: fixed;
    height: 32px;
    padding-top: 20px;

    &__name {
      font-family: "PT Sans Narrow";
      float: left;
      position: absolute;
      top: 0.8vw;
      left: 1vw;
      display: inline;
    }
    &__buttons{
      display: inline-flex;
      align-items: stretch;
      width: 25%;
      margin: 0;
      padding: 0px;
      float: right;
      justify-content: space-around;
      @media screen and (max-width: 900px){
        width: 35%;
      }
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

  i {
    display: table-cell;
    top: 0;
    transition: top ease 200ms;
  }

  i:hover {
    position: relative;
    color: #64ffda;
    top: -5px;
  }

  .router-link-active{
    color: #64ffda;
  }

</style>
