<template>
  <div>
    <iframe name="dummyframe" id="dummyframe" style="display: none;"></iframe>
    <div class="contact">
      <div class="contact__text">
        <div class="contact__text1">Contact Me</div>
        <div class="contact__text2">Have a question or want to work together?</div>
      </div>
      <div class="contact__form">
        <form action="https://mailthis.to/lakshit.contactme" method="POST" target="dummyframe" id="contact-me-form">
          <ul>
            <li><input type="text" name="name" placeholder="Your name" required></li>
            <li><input type="email" name="email" placeholder="Your Email" required></li>
            <li><textarea type="message" name="message" placeholder="Your Message" required></textarea></li>
            <button type="submit" value="Send" class="contact__button" @click="clear">SUBMIT</button>
          </ul>
        </form>
      </div>
    </div>
  </div>
</template>
<script>
  export default {
    components: {
    },
    methods:{
      clear: function(){
        alert("Thank you for getting in touch!")
        document.getElementById("contact-me-form").reset();
      }
    }
  }
</script>
<style lang="scss" scoped>

  ::placeholder {
    font-weight: 300;
    font-size: 15px;
  }

  .contact {
    color: #CCD6F6;
    width: 70%;
    height: 60%;
    position: absolute;
    top: 0;
    bottom: 0;
    left: 0;
    right: 0;
    margin: auto;

    &__form {
      padding-top: 20%;
      background: transparent;
      width: 70%;
      height: 80%;
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      margin: auto;
    }

    &__button {
      font-size: 1.5vw;
      border: 1px solid #64FFDA;
      color: #64FFDA;
      text-align: center;
      float: right;
      display: inline;
      padding: 5px;

      &:hover {
        color: #0a182f;
        background-color: #64FFDA;
      }
    }

    &__text {
      padding-bottom: 20px;
      width: 70%;
      position: absolute;
      top: 0;
      bottom: 0;
      left: 0;
      right: 0;
      margin: auto;
    }

    &__text1 {
      position: absolute;
      font-weight: bolder;
      font-size: 3.5vw;
      padding-bottom: 5px;
      display: inline-flex;
      z-index: 1;
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
    &__text1:hover {
      transition: all 2s cubic-bezier(0.000, 0.000, 0.230, 1);
      background-position: 100% 100%;
    }

    &__text2 {
      color: #64FFDA;
      font-size: 1.5vw;
      position: absolute;
      top: 4.5vw;
    }

  }
  ul {
    list-style-type: none;
    padding-left: 0px;
  }

  input {
    width: 94%;
    margin: 3px 0 3px 0;
    height: 2.5vw;
    border: none;
    background-color: #021024;
    padding-left: 3%;
    padding-right: 3%;
    color: #CCD6F6;
    font-size: 15px;
  }

  textarea {
    width: 94%;
    height: 10vw;
    border: none;
    background-color: #021024;
    padding-left: 3%;
    padding-right: 3%;
    color: #8892b0;
    font-size: 15px;
    padding-top: 1%;
    margin: 3px 0 8px;
  }
</style>
