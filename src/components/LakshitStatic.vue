<template>
  <div class="intro">
    <div class="intro-big">
      <div class="intro-big__one">Hi, my name is</div>
      <div class="intro-big__two">Lakshit Arora.</div>
      <div class="intro-big__three">I build things for the web</div>
    </div>
    <div class="intro-small">
      <div class="intro-small-info">
        I'm a software engineer based in Bengaluru, India.<br>
        I have a passion for web development and love <br> to create for web and mobile devices.
      </div>
    </div>
  </div>
</template>

<script>
  export default {
    name: "LakshitStatic.vue"
  }
</script>

<style scoped lang="scss">
  .intro {
    width: 70%;
    display: inline-block;
    margin: 0 auto;
    padding-top: 16%;
    padding-left: 10%;
    vertical-align: bottom;
  }

  .intro-big {
    font-weight: bolder;

    &__one {
      font-family: "Open Sans";
      color: #64FFDA;
      font-size: 1.5vw;
    }

    &__two {
      font-size: 6vw;
      display: inline-flex;
      color: #CCD6F6;
      text-decoration: none;
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

    &__two:hover {
      transition: all 2s cubic-bezier(0.000, 0.000, 0.230, 1);
      background-position: 100% 100%;
    }

    &__three {
      font-size: 5vw;
      color: #8892b0;
    }
  }

  .intro-small {
    font-family: "Open Sans";
    color: #8892b0;
    text-align: justify-all;
    padding-top: 2vw;
    font-size: 1.5vw;
  }

</style>