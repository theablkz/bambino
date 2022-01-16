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
      'https://images.ctfassets.net/hrltx12pl8hq/61DiwECVps74bWazF88Cy9/2cc9411d050b8ca50530cf97b3e51c96/Image_Cover.jpg?fit=fill&w=480&h=270',
      'https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRjq_N1ngW356j474_Uwe5g3GFf20a0-NK5-8emZk_cXc4eh6aAp24XbH6V_1edbS0P4L0&usqp=CAU',
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
  height: 700px;
}
</style>
