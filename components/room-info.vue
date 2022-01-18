<template>
  <div class='room-info'>
    <div class='room-texts'>
      <div>
        <h2 class='info-title'>{{roomInfo.title}}</h2>

        <ul class='room-info-list'>
          <li v-for='item in roomInfo.list'>{{item}}</li>
        </ul>
      </div>

      <div class='contact-buttons'>
        <a class='contact-button whatsapp whatsapp-des' :href='whatsapp' target='_blank'> <img class='contact-icon' src='~/assets/whatsapp.svg' alt=''> НАПИСАТЬ НАМ В WHATSAPP</a>
        <a class='contact-button whatsapp whatsapp-mob' :href='whatsappMob' target='_blank'> <img class='contact-icon' src='~/assets/whatsapp.svg' alt=''> НАПИСАТЬ НАМ В WHATSAPP</a>
        <a class='contact-button' href='tel: +7(707)1222020' target='_blank'> <img class='contact-icon' src='~/assets/call.svg' alt=''> ПОЗВОНИТЬ НАМ</a>
      </div>
    </div>
    <div class='images-box'>
      <div class="images" v-viewer>
        <video
          :src="roomVideo"
          controls

        >
          Sorry, your browser doesn't support embedded videos, but don't worry,
          you can <a :href="roomVideo">download it</a>
          and watch it with your favorite video player!
        </video>
        <img class='image' v-for="src in roomImages" :key="src" :src="src">
      </div>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'

import 'viewerjs/dist/viewer.css'
import Viewer from 'v-viewer'
Vue.use(Viewer)

const RoomText = [
  {
    title: 'Первый зал (150 кв.м.):',
    list: [
      'Мягкое игровое покрытие',
      '3х этажный лабиринт с винтовой горкой',
      'Развивающие игрушки, детские мотоциклы и толокары',
      'Аэро-хоккей',
      'Настольный футбол',
      'Батут',
      'Sony PlayStation',
      'Профессиональное караоке',
      'Бесплатный Wi-Fi',
      'Кухня: холодильник, микроволновка, чайник, посуда и приборы'
    ]
  },
  {
    title: 'Второй зал (100 кв.м.):',
    list: [
      'Мягкое игровое покрытие',
      '3х этажный лабиринт с винтовой горкой',
      'Развивающие игрушки, детские мотоциклы и толокары',
      'Аэро-хоккей',
      'Батут',
      'Sony PlayStation',
      'Профессиональное караоке',
      'Бесплатный Wi-Fi',
      'Кухня: холодильник, микроволновка, чайник, посуда и приборы'
    ]
  },
  {
    title: 'Третий зал (170 кв.м.):',
    list: [
      'Мягкое игровое покрытие',
      '3х этажный лабиринт с винтовой горкой',
      'Развивающие игрушки, детские мотоциклы и толокары',
      'Аэро-хоккей',
      'Батут',
      'Sony PlayStation',
      'Профессиональное караоке',
      'Бесплатный Wi-Fi',
      'Кухня: холодильник, микроволновка, чайник, посуда и приборы'
    ]
  }
]
const Images = [
  [
    '/room1/IMG_0565.jpeg',
    '/room1/IMG_0566.jpeg',
    '/room1/IMG_0568.jpeg',
    '/room1/IMG_0573.jpeg',
    '/room1/IMG_0579.jpeg',
    '/room1/IMG_0581.jpeg',
    '/room1/IMG_0582.jpeg',
    '/room1/IMG_0584.jpeg',
    '/room1/IMG_0588.jpeg',
    '/room1/IMG_0591.jpeg',
    '/room1/IMG_0595.jpeg',
    '/room1/IMG_0675.jpeg',
  ],
  [
    '/room2/IMG_0138.jpeg',
    '/room2/IMG_0598.jpeg',
    '/room2/IMG_0600.jpeg',
    '/room2/IMG_0607.jpeg',
    '/room2/IMG_0608.jpeg',
    '/room2/IMG_0612.jpeg',
    '/room2/IMG_0615.jpeg',
    '/room2/IMG_0616.jpeg',
    '/room2/IMG_0618.jpeg',
    '/room2/IMG_0620.jpeg',
    '/room2/IMG_0622.jpeg',
  ],
  [
    '/room3/IMG_0643.jpeg',
    '/room3/IMG_0644.jpeg',
    '/room3/IMG_0645.jpeg',
    '/room3/IMG_0646.jpeg',
    '/room3/IMG_0648.jpeg',
    '/room3/IMG_0649.jpeg',
    '/room3/IMG_0651.jpeg',
    '/room3/IMG_0652.jpeg',
    '/room3/IMG_0653.jpeg',
    '/room3/IMG_0657.jpeg',
    '/room3/IMG_0660.jpeg',
    '/room3/IMG_0663.jpeg',
  ]
]
const Viedeos = [
  '/room1/1й зал 150кв.м.mp4',
  '/room2/2й зал 100кв.м.mp4',
  '/room3/3й зал 170кв.м.mp4',
]

export default {
  name: 'room-info',
  props: ['room'],
  computed: {
    roomInfo(){
      return RoomText[this.room - 1]
    },
    roomImages(){
      return Images[this.room - 1]
    },
    roomVideo(){
      return Viedeos[this.room - 1]
    },
    whatsapp() {
      return  `https://web.whatsapp.com/send?phone=77071222020`
    },
    whatsappMob(){
      return `https://wa.me/77071222020`
    }
  }
}
</script>

<style lang='scss' scoped>


.room-texts {
  display: flex;
  justify-content: space-between;
  padding: 48px 16px 72px;
  max-width: 1000px;
  margin: auto;

  .info-title {
    margin-bottom: 24px;
  }
  .room-info-list {
    list-style: disc inside none;
    line-height: 1.3;
  }
  .contact-buttons {
    margin-top: 48px;

    .contact-button {
      margin: auto auto 16px auto;
      text-decoration: none;
      padding: 12px 24px;
      color: white;
      background: rgba(238, 50, 57, 1);
      border-radius: 20px;
      display: flex;
      align-items: center;
      width: 215px;
      box-shadow: 0 3px 6px rgba(0, 0, 0, 0.16), 0 3px 6px rgba(0, 0, 0, 0.23);
      transition: all 0.3s cubic-bezier(.25, .8, .25, 1);

      &:hover {
        box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25), 0 10px 10px rgba(0, 0, 0, 0.22);
      }

      &.whatsapp-des {
        @media screen and (max-width: 1000px) {
          display: none;
        }
      }

      &.whatsapp-mob {
        @media screen and (min-width: 1000px) {
          display: none;
        }
      }

      .contact-icon {
        width: 24px;
        height: auto;
        margin-right: 8px;
      }
    }
  }

}

.images-box {
  padding: 48px 16px 72px;
  max-width: 1000px;
  margin: auto;
  .images {
    display: grid;
    grid-template-columns: 1fr 1fr 1fr 1fr;
    gap: 16px;
    .image {
      width: 100%;
      height: 170px;
      object-fit: cover;
      &:hover {
        cursor: pointer;
      }
    }
  }
}

video {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

</style>
