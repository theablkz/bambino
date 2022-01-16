<template>
  <div>
    <header-component />
    <room-head />
    <room-info :room='room' />
    <our-halls />
    <footer-component />
  </div>
</template>

<script>
import HeaderComponent from '../../components/header-component'
import OurHalls from '../../components/our-halls'
import FooterComponent from '../../components/footer-component'
import RoomHead from '../../components/room-head'
import RoomInfo from '../../components/room-info'
export default {
  name: 'rooms',
  components: { RoomInfo, RoomHead, FooterComponent, OurHalls, HeaderComponent },
  computed: {
    room(){
      return this.$route.params.id
    }
  }
}
</script>

<style scoped>

</style>
