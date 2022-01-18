<template>
  <div>
    <client-only>
      <VueSlickCarousel v-bind="settings">
        <div
          v-for="item in otherBuilds"
          :href="item.link"
          target="_blank"
          :key="item.id"
        >
          <img class="apartment-image" :src="item" alt="" />
        </div>
      </VueSlickCarousel>
    </client-only>
  </div>
</template>

<script>
import VueSlickCarousel from 'vue-slick-carousel'
import 'vue-slick-carousel/dist/vue-slick-carousel.css'
// optional style for arrows & dots
import 'vue-slick-carousel/dist/vue-slick-carousel-theme.css'
export default {
  components: { VueSlickCarousel },
  data: () => ({
    otherBuilds: [
      '/gallery/IMG_4969.JPG',
      '/gallery/IMG_5051.JPG',
      '/gallery/IMG_5067.JPG',
      '/gallery/IMG_5069.JPG',
      '/gallery/IMG_5076.JPG',
      '/gallery/IMG_5100.JPG',
      '/gallery/IMG_5940.JPG',
      '/gallery/IMG_7848.JPG',
      '/gallery/IMG_8909.JPG',
      '/gallery/IMG_9133.JPG',
      '/gallery/IMG_9173.JPG',
      '/gallery/IMG_9320.JPG',
      '/gallery/IMG_9348.JPG',
    ],
    settings: {
      dots: false,
      arrows: true,
      infinite: true,
      speed: 500,
      initialSlide: 0,
      edgeFriction: 0.35,
      slidesToShow: 1,
      slidesToScroll: 1,
    },
  }),
}
</script>

<style>
.apartment-image {
  width: 100%;
  object-fit: cover;
  height: 850px;
}
</style>
