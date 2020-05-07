<template>
  <div class="navbar">
    <ul>
      <li><a href="https://github.com/lakshitarora14" target="_blank">
        <i class="fab fa-github fa-lg"></i>
      </a></li>
      <li><a href="https://www.linkedin.com/in/lakshitarora/" target="_blank">
        <i class="fab fa-linkedin-in fa-lg"></i>
      </a></li>
      <li><a href="https://www.instagram.com/lakshit__arora/" target="_blank">
        <i class="fab fa-instagram fa-lg"></i>
      </a></li>
      <li><a href="https://twitter.com/lakshitarora14" target="_blank">
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
    background: transparent;
  }

  .line {
    height: auto;
    min-height: 12vw;
    border-right: 2px solid #8892b0;
    display: inline-block;
    position: absolute;
    right: 50%;
    bottom: 0;
  }

  .navbar {
    position: absolute;
    min-height: 100%;
    width: 70px;
    left: 0;
  }

  i {
    position: relative;
    height: 45px;
    width: 45px;
    background:transparent;
  }

  a {
    color: #A8B2D1;
    text-decoration: none;
  }
  a:hover{
    color: #64FFDA;
  }

  li:hover > li{
    background:transparent;
    margin-left: 10px;
    float: left;
    -webkit-transition: margin 100ms ease-out;
    -moz-transition: margin 100ms ease-out;
    -o-transition: margin 100ms ease-out;
  }

  ul {
    list-style-type: none;
    position: absolute;
    right: 0;
    bottom: 11vw;
    display: inline;
  }

</style>