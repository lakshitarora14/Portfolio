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

  .line {
    height: 150px;
    border-right: 2px solid #8892b0;
    width: 50%;
    z-index: 1;
    position: absolute;
    bottom: 0;
  }

  .navbar {
    position: relative;
    border: 2px solid red;
    min-height: 100vh;
    box-sizing: border-box;
    height: auto;
    width: 60px;
    float: right;
    padding-right: 20px;
  }
</style>