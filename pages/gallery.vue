<template>
  <div>
    <header-component />
    <our-rooms />
    <slider />
    <our-videos />
    <our-halls />
    <footer-component />
  </div>
</template>

<script>
import HeaderComponent from '../components/header-component'
import OurRooms from '../components/our-rooms'
import Slider from '../components/slider'
import OurVideos from '../components/our-videos'
import OurHalls from '../components/our-halls'
import FooterComponent from '../components/footer-component'
export default {
  name: 'gallery',
  components: { FooterComponent, OurHalls, OurVideos, Slider, OurRooms, HeaderComponent }
}
</script>

<style scoped>

</style>
