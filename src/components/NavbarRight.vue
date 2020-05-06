<template>
  <div class="navbar">
    <div class="email">
      <a href="https://mail.google.com/mail/?view=cm&fs=1&to=lakshitarora14@gmail.com">
        lakshitarora14@gmail.com
      </a>
    </div>
    <div class="line"></div>
  </div>
</template>

<script>
  export default {
    name: "NavbarRight.vue"
  }
</script>

<style scoped lang="scss">
  * {
    padding: 0px;
    margin: 0px;
  }
  a {
    color: #A8B2D1;
    text-decoration: none;
  }

  a:hover {
    color: #64FFDA;
  }
  .email{
    font-family:"Montserrat";
    transform: rotate(90deg);
    font-size: 15px;
    margin-top: 27vw;
    margin-left: 2vw;
  }
  .email:hover{
    padding-top: 7px;
    -webkit-transition: margin 100ms ease-out;
    -moz-transition: margin 100ms ease-out;
    -o-transition: margin 100ms ease-out;
  }
  .line {
    height: 12vw;
    border-right: 2px solid #8892b0;
    width: 50%;
    z-index: 1;
    position: absolute;
    bottom: 0;
  }

  .navbar {
    position: relative;
    min-height: 100vh;
    box-sizing: border-box;
    height: auto;
    width: 60px;
    float: right;
    padding-right: 20px;
  }
</style>