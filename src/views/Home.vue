<template>
  <div class="home">
    <NavbarLeft></NavbarLeft>
    <navbar-right></navbar-right>
    <LakshitStatic></LakshitStatic>
    <ContactButton></ContactButton>
  </div>
</template>

<script>
  import NavbarLeft from '../components/NavbarLeft'
  import NavbarRight from '../components/NavbarRight'
  import LakshitStatic from '../components/LakshitStatic'
  import ContactButton from '../components/ContactButton'

  export default {
    name: 'Home',
    components: {
      NavbarLeft, NavbarRight,LakshitStatic,ContactButton
    }
  }
</script>
