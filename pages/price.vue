<template>
  <div>
    <header-component />
    <arenda />
    <prices-info />
    <footer-component />
  </div>
</template>

<script>
import HeaderComponent from '../components/header-component'
import FooterComponent from '../components/footer-component'
import Arenda from '../components/arenda'
import PricesInfo from '../components/prices'
export default {
  name: 'price',
  components: { PricesInfo, Arenda, FooterComponent, HeaderComponent }
}
</script>

<style scoped>

</style>
