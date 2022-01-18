<template>
  <div class="room-head" :class="`room-${room}`">
    <div class="head-content">
      <h1 class='head-title'>Квест комнаты и Шоу программы</h1>

      <div class='room-box'>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'quest-head',
  computed: {
    roomImage(){
      const imagesUrl = ['10.png', '11.png', '12.png']
      return imagesUrl[0]
    },
    room() {
      return 4
    }
  }
}
</script>

<style lang="scss" scoped>
.room-head {
  min-height: 600px;
  display: flex;
  align-items: center;
  justify-content: center;

  .head-content {
    .head-title {
      color: white;
      font-size: 52px;
      margin-bottom: 32px;
    }
    .room-box {
      display: grid;
      grid-template-columns: auto auto;
      gap: 24px;
      align-items: center;
      justify-content: center;
      .room-des {
        color: white;
        font-size: 58px;
      }
    }
    .hall-scheme {
      width: 200px;
      height: auto;

    }
  }






  &.room-1 {
    background: linear-gradient(rgba(255, 0, 0, 0.45), rgba(255, 0, 0, 0.45)),
    url('/3-1026x616.jpg') no-repeat center center;
    background-size: cover;
  }
  &.room-2 {
    background: linear-gradient(rgba(39,85,122, 0.45), rgba(39,85,122, 0.45)),
    url('/3-1026x616.jpg') no-repeat center center;
    background-size: cover;
  }
  &.room-3 {
    background: linear-gradient(rgba(0, 124, 185, 0.45), rgba(0, 124, 185, 0.45)),
    url('/3-1026x616.jpg') no-repeat center center;
    background-size: cover;
  }
  &.room-4 {
    background: linear-gradient(rgba(0, 124, 185, 0.45), rgba(0, 124, 185, 0.45)),
    url('/quest/г 4.JPG') no-repeat center center;
    background-size: cover;
  }
}
</style>
