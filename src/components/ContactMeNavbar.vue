<template>
  <div class="nav">
    <div class="center">Built with
      <div class="heart"><i class="fas fa-heart"></i></div>
      and css
    </div>
    <div class="right">© {{ year }} Lakshit Arora</div>
  </div>
</template>

<script>
  export default {
    name: "ContactMeNavbar",
    data() {
      return {
        year:new Date().getFullYear(),
      }
    },
  }
</script>
<style scoped lang="scss">
  @keyframes beat {
    to {
      transform: scale(1.5);
    }
  }

  * {
    background-color: #091426;
    z-index: 1;
  }

  .center {
    padding-top: 12px;
    padding-left: 2.6%;
    float: left;
    display: flex;
    vertical-align: middle;
    text-align: center;
  }

  .heart {
    padding-left: 5px;
    padding-right: 5px;
    color: red;
    cursor: pointer;

    :hover {
      background: transparent;
      animation: beat .25s infinite alternate;
      transform-origin: center;
    }
  }

  .right {
    position: absolute;
    right: 3%;
    margin-top: 20px;
    font-size: 12px;

    :hover {
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