<template>
  <div class="home">
    <NavbarLeft></NavbarLeft>
    <navbar-right></navbar-right>
    <LakshitStatic></LakshitStatic>
    <ContactButton></ContactButton>
    <ContactMeNavbar></ContactMeNavbar>
  </div>
</template>

<script>
  import NavbarLeft from '../components/NavbarLeft'
  import NavbarRight from '../components/NavbarRight'
  import LakshitStatic from '../components/LakshitStatic'
  import ContactButton from '../components/ContactButton'
  import ContactMeNavbar from '../components/ContactMeNavbar'

  export default {
    name: 'Home',
    components: {
       NavbarRight,LakshitStatic,ContactButton,ContactMeNavbar,NavbarLeft
    }
  }
</script>
