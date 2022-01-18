<template>
  <div class='header'>
    <div class='header-content'>
      <nuxt-link to='/'>
        <img src='~/assets/logo.png'  alt='logo' class='logo'>
      </nuxt-link>
      <ul class='header-links'>
        <li><nuxt-link to='/contacts'>НАШИ ЗАЛЫ</nuxt-link></li>
        <li><nuxt-link to='/price'>ЦЕНЫ</nuxt-link></li>
        <li><nuxt-link to='/gallery'>ГАЛЕРЕЯ</nuxt-link></li>
        <li><nuxt-link to='/quests'>КВЕСТЫ</nuxt-link></li>
        <li><nuxt-link to='/contacts'>КОНТАКТЫ</nuxt-link></li>
      </ul>
      </div>
  </div>
</template>

<script>
export default {
  name: 'header-component'
}
</script>

<style lang='scss' scoped>
.header {
  background: rgb(13,121,177);
  background: linear-gradient(132deg, rgba(13,121,177,1) 8%, rgba(206,60,74,1) 77%, rgba(238,50,57,1) 100%);
  min-height: 100px;
  .header-content {
    max-width: 1000px;
    padding: 16px 24px 50px 16px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: flex-end;

    .logo {
      width: 200px;
      height: auto;
    }
    .header-links {
      text-decoration: none;
      display: flex;
      gap: 24px;
      justify-content: space-around;
      a {
        text-decoration: none;
        font-weight: 500;
        color: white;
      }
    }

  }
}


</style>
