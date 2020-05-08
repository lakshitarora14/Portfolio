<template>
  <div>
    <ContactMeNavbar></ContactMeNavbar>
    <navbar-right></navbar-right>
    <navbar-left></navbar-left>
    <div class="about">
      <div class="about__left">
        <div class="about__heading">
          About Me
        </div>
        <div class="about__content">
          Hello! I'm Lakshit, a software engineer based in Bengaluru, India.
          <br><br>
          I enjoy creating things that live on the internet, whether that be
          websites, applications, or anything in between. My goal is to always
          build products that provide pixel-perfect, performant experiences.
          <br><br>
          I am currently working at <a href="https://www.coviam.com/" target="_blank">Coviam Technologies</a> where I
          work on a wide variety of interesting and meaningful projects on a daily basis.
          <br><br>
          Here are a few technologies I've been working with recently:
          <ul class="ul-left">
            <li>Springboot</li>
            <li>Java</li>
            <li>HTML & (S)CSS</li>
          </ul>
          <ul class="ul-right">
            <li>vue.js</li>
            <li>JavaScript (ES6+)</li>
            <li>NoSQL</li>
          </ul>
          <br><br>
          Visit my <a href="linkedin.com/in/lakshitarora" target="_blank">linkedin</a>
          profile for more details or just
          <router-link to="/contact-me" class="route"> contact me.</router-link>
        </div>
      </div>
      <div class="about__right">
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    components: {
      NavbarRight, NavbarLeft, ContactMeNavbar
    }
  }
  import NavbarLeft from '../components/NavbarLeft'
  import NavbarRight from '../components/NavbarRight'
  import ContactMeNavbar from '../components/ContactMeNavbar'
</script>
<style scoped lang="scss">
  @import "../assets/variables";

  a {
    text-decoration: none;
    color: $lightColor;
  }

  ul {
    display: inline-block;
    width: 42%;
    padding: 20px;
  }

  li {

  }

  .about {
    color: $textColorDark;
    display: inline-flex;
    padding: 8%;
    height: 70%;
    font-size: 18px;

    &__left {
      border: 2px solid red;
      width: 50%;
      float: left;
    }

    &__right {
      border: 2px solid yellow;
      width: 50%;
      float: right;
    }

    &__heading {
      font-weight: 700;
      color: $textColor;
      font-size: 50px;
      padding-bottom: 2vw;
      display: inline-flex;
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

    &__heading:hover {
      transition: all 2s cubic-bezier(0.000, 0.000, 0.230, 1);
      background-position: 100% 100%;
    }

    &__content {
      text-align: justify;
    }
  }
</style>