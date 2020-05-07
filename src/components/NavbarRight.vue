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
    background: transparent;
  }
  a {
    color: #A8B2D1;
    text-decoration: none;
  }

  a:hover {
    color: #64FFDA;
  }
  .email{
    position: absolute;
    transform: rotate(90deg);
    right: 0;
    bottom: 20vw;
    font-size: 15px;
    margin-right: -5vw;
  }
  .email:hover{
    padding-top: 7px;
    padding-left: 7px;
    -webkit-transition: margin 100ms ease-out;
    -moz-transition: margin 100ms ease-out;
    -o-transition: margin 100ms ease-out;
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
    right: 0;
  }
</style>