<template>
  <div class="navbar">
    <ul>
      <li><a href="">
        <i class="fab fa-github"></i>
      </a></li>
      <li><a href="">
        <i class="fab fa-linkedin-in"></i>
      </a></li>
      <li><a href="">
        <i class="fab fa-instagram"></i>
      </a></li>
      <li><a href="">
        <i class="fab fa-twitter"></i>
      </a></li>
    </ul>
  </div>
</template>

<script>
  export default {
    name: "NavbarLeft.vue"
  }
</script>

<style scoped lang="scss">
  .navbar{
    margin-top: 100px;
    background-color: white;
    height: 100%;
    width: 50px;
    float: left;
  }
  i{
    color: white;
  }
  ul{
    list-style-type:none;
  }

</style>