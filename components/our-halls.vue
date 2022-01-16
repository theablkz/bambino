<template>
  <div class="our-halls">
      <div class="our-halls-block-content">
          <h1 class="our-halls-block-title">НАШИ ЗАЛЫ</h1>
          <div class="our-halls-block-contents">
            <nuxt-link to="/room/1" class="our-halls-block-hall hall-1">
                <img class="hall-scheme" src="~/assets/10.png" alt="">
                <h1>ЗАЛ #1</h1>
                <img class="hall-arrow" src="~/assets/arrow-compress.png" alt="">
            </nuxt-link>
             <nuxt-link to="/room/2" class="our-halls-block-hall hall-2">
                <img class="hall-scheme" src="~/assets/11.png" alt="">
                <h1>ЗАЛ #2</h1>
                <img class="hall-arrow" src="~/assets/arrow-compress.png" alt="">
            </nuxt-link>
             <nuxt-link to="/room/3" class="our-halls-block-hall hall-3">
                <img class="hall-scheme" src="~/assets/12.png" alt="">
                <h1>ЗАЛ #3</h1>
                <img class="hall-arrow" src="~/assets/arrow-compress.png" alt="">
            </nuxt-link>
          </div>
      </div>

  </div>
</template>

<script>
export default {
    name: 'our-halls'

}
</script>

<style lang="scss" scoped>
.our-halls {
   background-color: white;
  min-height: 300px;
  .our-halls-block-content {
    max-width: 1000px;
    padding: 50px 24px 50px 16px;
    margin: auto;
 .our-halls-block-title {
      font-weight: bold;
      color: rgba(238,50,57,1);
      text-align: center;
      font-size: 28px;
      margin-bottom: 32px;
    }

    .our-halls-block-contents {
      display: grid;
      grid-template-columns: 1fr 1fr 1fr;
      gap: 48px;
      .our-halls-block-hall {
          border-radius: 40% / 4%;

          padding: 48px 16px 24px 16px;
          text-decoration: none;
          color: inherit;
          &.hall-1 {
              background-color:rgba(238,50,57,1);
          }
          &.hall-2 {
              background-color:#27557a;
          }
          &.hall-3 {
              background-color:#007cb9;
          }
          h1 {
              font-size:32px;
              font-weight: bold;
                color: rgba(0,0,0,0.6);
                text-align: center;

          }
            .hall-scheme {
                width: 220px;
                height: auto;
                margin: auto auto 24px auto;
                display: block;
            }
            .hall-arrow {
                display: block;
                margin: auto 0 auto auto;
            }
      }
    }

  }
}

</style>
