<template>
  <div class="our-videos">
    <div class="our-videos-block-content">
      <h1 class="our-videos-block-title">ВИДЕО</h1>
      <div class="our-videos-block-videos">
        <video
          src="/room1/1й зал 150кв.м.mp4"
          controls

        >
          Sorry, your browser doesn't support embedded videos, but don't worry,
          you can <a href="/room1/1й зал 150кв.м.mp4">download it</a>
          and watch it with your favorite video player!
        </video>
        <video
          src="/room2/2й зал 100кв.м.mp4"
          controls

        >
          Sorry, your browser doesn't support embedded videos, but don't worry,
          you can <a href="/room2/2й зал 100кв.м.mp4">download it</a>
          and watch it with your favorite video player!
        </video>
        <video
          src="/room3/3й зал 170кв.м.mp4"
          controls

        >
          Sorry, your browser doesn't support embedded videos, but don't worry,
          you can <a href="/room3/3й зал 170кв.м.mp4">download it</a>
          and watch it with your favorite video player!
        </video>


      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.our-videos {
  background-image: url('~/assets/bg1.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  min-height: 300px;
  .our-videos-block-content {
    max-width: 1000px;
    padding: 50px 24px 50px 16px;
    margin: auto;
    .our-videos-block-title {
      font-weight: bold;
      color: white;
      text-align: center;
      font-size: 22px;
      margin-bottom: 32px;
    }
    .our-videos-block-videos {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 32px;
    }
  }
}
video {
    width: 100%;
    height: 300px;
}
</style>
