<template>
  <div>
    <header-component />
    <our-halls />
    <footer-component />
  </div>
</template>

<script>
import HeaderComponent from '../components/header-component'
import OurHalls from '../components/our-halls'
import FooterComponent from '../components/footer-component'
export default {
  name: 'contacts',
  components: { FooterComponent, OurHalls, HeaderComponent }
}
</script>

<style scoped>

</style>
