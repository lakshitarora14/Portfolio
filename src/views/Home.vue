<template>
  <div class="home">
    <LakshitStatic></LakshitStatic>
    <ContactButton></ContactButton>
  </div>
</template>

<script>
  import LakshitStatic from '../components/LakshitStatic'
  import ContactButton from '../components/ContactButton'

  export default {
    name: 'Home',
    components: {
      LakshitStatic, ContactButton,
    }
  }
</script>
