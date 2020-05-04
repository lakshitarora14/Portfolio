<template>
  <div class="home">
    <NavbarLeft></NavbarLeft>
    <navbar-right></navbar-right>
  </div>
</template>

<script>
  import NavbarLeft from '../components/NavbarLeft'
  import NavbarRight from '../components/NavbarRight'

  export default {
    name: 'Home',
    components: {
      NavbarLeft, NavbarRight
    }
  }
</script>
