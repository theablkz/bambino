<template>
  <div>
    <main-page />
    <our-rooms />
    <slider />
    <our-videos />
    <our-halls />
    <footer-component />

  </div>
</template>

<script>
import FooterComponent from '../components/footer-component.vue'
import HeaderComponent from '../components/header-component'
import OurHalls from '../components/our-halls.vue'
import OurRooms from '../components/our-rooms'
import OurVideos from '../components/our-videos.vue'
import Slider from '../components/slider.vue'
import MainPage from '../components/main-page'
export default {
  name: 'IndexPage',
  components: { MainPage, OurRooms, HeaderComponent,FooterComponent, Slider, OurVideos, OurHalls },
}
</script>,

