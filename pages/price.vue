<template>
  <div>
    <header-component />
    <arenda />
    <footer-component />
  </div>
</template>

<script>
import HeaderComponent from '../components/header-component'
import FooterComponent from '../components/footer-component'
import Arenda from '../components/arenda'
export default {
  name: 'price',
  components: { Arenda, FooterComponent, HeaderComponent }
}
</script>

<style scoped>

</style>
