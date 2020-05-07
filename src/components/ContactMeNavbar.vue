<template>
  <div class="nav">
  <div class="center">Built with <div class="heart"><i class="fas fa-heart"></i></div> and css</div>
    <div class="right"><a href="https://github.com/lakshitarora14/Portfolio" target="_blank"> Source code</a></div>
  </div>
</template>

<script>
  export default {
    name: "ContactMeNavbar.vue"
  }
</script>

<style scoped lang="scss">
  a{
    text-decoration: none;
    color: #CCD6F6;
  }
  @keyframes beat{
    to { transform: scale(1.5); }
  }
  *{
    background-color: #091426;

  }
  .center{
    padding-top: 12px;
    padding-left: 8%;
    float: left;
    display: flex;
    vertical-align: middle;
    text-align: center;
  }
  .heart{
    padding-left: 5px;
    padding-right: 5px;
    color: red;
    cursor: pointer;
    :hover{
    background: transparent;
    animation: beat .25s infinite alternate;
    transform-origin: center;
  }
  }
  .right{
    float: right;
    margin-right: 8%;
    cursor: pointer;
    margin-top: 12px;
    :hover{
      color: #64FFDA;
    }
  }
  .nav {
    display: table;
    height: 50px;
    width: 100%;
    color: #CCD6F6;
    font-size: 20px;
    position: absolute;
    bottom: 0;
    font-weight: 300;
  }
</style>