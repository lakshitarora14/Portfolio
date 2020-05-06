<template>
  <div class="navbar">
    <ul>
      <li><a href="https://github.com/lakshitarora14">
        <i class="fab fa-github fa-lg"></i>
      </a></li>
      <li><a href="https://www.linkedin.com/in/lakshitarora/">
        <i class="fab fa-linkedin-in fa-lg"></i>
      </a></li>
      <li><a href="https://www.instagram.com/lakshit__arora/">
        <i class="fab fa-instagram fa-lg"></i>
      </a></li>
      <li><a href="https://twitter.com/lakshitarora14">
        <i class="fab fa-twitter fa-lg"></i>
      </a></li>
    </ul>
    <div class="line"></div>
  </div>
</template>

<script>
  export default {
    name: "NavbarLeft.vue"
  }
</script>

<style scoped lang="scss">
  * {
    padding: 0px;
    margin: 0px;
  }

  .line {
    height: 150px;
    border-right: 2px solid #8892b0;
    width: 50%;
    bottom: 0;
    position: absolute;
  }

  .navbar {
    min-height: 100vh;
    box-sizing: border-box;
    height: auto;
    width: 60px;
    float: left;
    position: relative;
    padding-left: 20px;
  }

  i {
    height: 45px;
    width: 45px;
    background:transparent;
  }

  i:hover {
    background:transparent;
    margin-left: 5px;
    padding-right: 2px;
    float: left;
    -webkit-transition: margin 100ms ease-out;
    -moz-transition: margin 100ms ease-out;
    -o-transition: margin 100ms ease-out;
  }

  a {
    color: #A8B2D1;
    text-decoration: none;
  }

  a:hover {
    color: #64FFDA;
  }

  ul {
    margin-top: 390px;
    list-style-type: none;
    padding-left: 50%;
  }

</style>