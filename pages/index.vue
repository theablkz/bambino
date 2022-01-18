<template>
  <div>
    <main-page />
    <our-halls />
    <our-services />
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
import OurServices from '../components/our-services'
export default {
  name: 'IndexPage',
  components: { OurServices, MainPage, OurRooms, HeaderComponent,FooterComponent, Slider, OurVideos, OurHalls },
}
</script>,

