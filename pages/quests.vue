<template>
  <div>
    <header-component />
    <quest-head />
    <quest />
    <our-halls />
    <footer-component />
  </div>
</template>

<script>

import Quest from '../components/quest'
import HeaderComponent from '../components/header-component'
import OurHalls from '../components/our-halls'
import FooterComponent from '../components/footer-component'
import QuestHead from '../components/quest-head'
export default {
  name: 'quests',
  components: { QuestHead, FooterComponent, OurHalls, HeaderComponent, Quest }
}
</script>

<style scoped>

</style>
