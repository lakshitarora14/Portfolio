<template>
  <div class="navbar">
    <div class="email">
      <a href="https://mail.google.com/mail/?view=cm&fs=1&to=lakshitarora14@gmail.com" target="_blank">
        contact@lakshit.tech
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
    left: 0;
    transition: left ease 200ms;
  }

  a:hover {
    position: relative;
    color: #64ffda;
    left: -5px;
  }

  .email {
    position: absolute;
    transform: rotate(90deg);
    right: -0.7vw;
    bottom: 21vw;
    font-size: 15px;
    margin-right: -5vw;
    letter-spacing: 3px;
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