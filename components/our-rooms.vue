<template>
  <div class='our-rooms-block'>
      <div class='our-rooms-block-content'>
          <h1 class='our-rooms-block-title'>ФОТО</h1>
        <div class='our-rooms-block-photos'>
          <nuxt-link class='our-rooms-block-photo' to='/'>
            <img class='photo-room' src='~/assets/rooms/4-492x295.jpg' alt=''>
            <h2 class='photo-title'>ЗАЛ #1</h2>
            <img class='arrow-right' src='~/assets/13.png' alt=''>
          </nuxt-link>
          <nuxt-link class='our-rooms-block-photo' to='/'>
            <img class='photo-room' src='~/assets/rooms/3-676x406.jpg' alt=''>
            <h2 class='photo-title'>ЗАЛ #2</h2>
            <img class='arrow-right' src='~/assets/13.png' alt=''>
          </nuxt-link>
          <nuxt-link class='our-rooms-block-photo' to='/'>
            <img class='photo-room' src='~/assets/rooms/2-676x406.jpg' alt=''>
            <h2 class='photo-title'>ЗАЛ #3</h2>
            <img class='arrow-right' src='~/assets/13.png' alt=''>
          </nuxt-link>
        </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'our-rooms'
}
</script>

<style lang='scss' scoped>
.our-rooms-block {
  background-image: url("~/assets/bg1.png");
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  min-height: 300px;
  .our-rooms-block-content {
    max-width: 1000px;
    padding: 50px 24px 50px 16px;
    margin: auto;
    .our-rooms-block-title {
      font-weight: bold;
      color: white;
      text-align: center;
      font-size: 22px;
      margin-bottom: 32px;
    }
    .our-rooms-block-photos {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;

      gap: 32px;
    }
    .our-rooms-block-photo {
      text-decoration: none;
      .photo-room {
        width: 100%;
        height: auto;
      }
      .photo-title {
        color: white;
        font-size: 28px;
        text-align: center;
        margin-top: 24px;
        margin-bottom: 24px;
      }
      .arrow-right {
        display: block;
        margin-left: auto;
      }
    }
  }
}
</style>
