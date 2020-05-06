<template>
  <div>
    <br>
    <router-link to="/contact-me" class="route">
      <div class="contact">
        CONTACT ME
      </div>
    </router-link>
  </div>
</template>

<script>
  export default {
    name: "ContactButton.vue"
  }
</script>

<style scoped lang="scss">
  *{
    font-family: "Montserrat";
    font-weight: 300;
    letter-spacing: 2px;
  }
  .contact{
    border: 1px solid #64FFDA;
    color: #64FFDA;
    height: 35px;
    width: 150px;
    margin-left: 15%;
    display: flex;
    &:hover{
      color: #0a182f;
      background-color: #64FFDA;
    }
  }
  a{
    text-decoration: none;
  }

</style>