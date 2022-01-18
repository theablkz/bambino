<template>
  <div class="room-info">
    <div class="room-texts">
      <div>
        <h2 class="info-title">Квест комнаты</h2>
        <p class='info-des'>
          Хотите попасть в загадочный городок Гравити фолз или в реальную игру
          Майнкрафт?
        </p>
        <p class='info-des info-des--red'>
          Тогда вам стоит посетить наши квест- комнаты в «волшебном подземелье»!
        </p>
        <p class='info-des'>
          Сам Квест технологичный и красочный, интересный для тинейджеров. На
          него использовано более 150 кв.м метров баннеров, для создания
          атмосферы нахождения в игре или мультике.
        </p>
        <p class='info-des'>
          Логический поиск артефактов и обязательный момент активити, где детям
          нужно стрелять, кидать и проявлять смекалку, проходит в фоновом
          музыкальном и световом сопровождении по тематике, и антуражу квеста.
          Все задания разнообразные и интересные, направленные на саморазвитие и
          самовыражение подростка.
        </p>


        <h2 class="info-title info-title-price">Прайс</h2>
        <h2 class="info-title">Квест комнаты (от 6 до 12 лет):</h2>
        <ul>
          <li>
            <p class="info-des">
              Гравити Фолз (от 3-6 чел, от 40мин до 60 мин) - <span>12 000 тг</span> + 1
              000 на каждого след. ребенка (max до 13 детей)
            </p>
          </li>
          <li>
            <p class="info-des mb-4">
              Майнкрафт (от 3-6 чел, от 40мин до 60 мин) - <span>14 000 тг</span> + 1 000
              на каждого след. ребенка (max до 13 детей)
            </p>
          </li>
        </ul>

        <!--        <ul class='room-info-list'>-->
        <!--          <li v-for='item in roomInfo.list'>{{item}}</li>-->
        <!--        </ul>-->
      </div>

      <div class="contact-buttons">
        <a
          class="contact-button whatsapp whatsapp-des"
          :href="whatsapp"
          target="_blank"
        >
          <img class="contact-icon" src="~/assets/whatsapp.svg" alt="" />
          НАПИСАТЬ НАМ В WHATSAPP</a
        >
        <a
          class="contact-button whatsapp whatsapp-mob"
          :href="whatsappMob"
          target="_blank"
        >
          <img class="contact-icon" src="~/assets/whatsapp.svg" alt="" />
          НАПИСАТЬ НАМ В WHATSAPP</a
        >
        <a class="contact-button" href="tel: +7(707)1222020" target="_blank">
          <img class="contact-icon" src="~/assets/call.svg" alt="" /> ПОЗВОНИТЬ
          НАМ</a
        >
      </div>
    </div>
    <div class="images-box">
      <div class="images" v-viewer>
        <img class="image" v-for="src in roomImages" :key="src" :src="src" />
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
      'Кухня: холодильник, микроволновка, чайник, посуда и приборы',
    ],
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
      'Кухня: холодильник, микроволновка, чайник, посуда и приборы',
    ],
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
      'Кухня: холодильник, микроволновка, чайник, посуда и приборы',
    ],
  },
]
const Images = [
  '/quest/г 1.JPG',
  '/quest/г 2.JPG',
  '/quest/г 3.JPG',
  '/quest/г 4.JPG',
  '/quest/г 5.JPG',
  '/quest/г 6.jpg',
  '/quest/г 7.jpg',
  '/quest/м 1.jpg',
  '/quest/м 2.jpg',
  '/quest/м 3.jpg',
  '/quest/м 4.jpg',
  '/quest/м 5.jpg',
  '/quest/м 6.jpg',
  '/quest/р 1.jpg',
  '/quest/р 2.jpg',
]

export default {
  name: 'quest',
  computed: {
    roomInfo() {
      return RoomText[0]
    },
    roomImages() {
      return Images
    },
    whatsapp() {
      return `https://web.whatsapp.com/send?phone=77071222020`
    },
    whatsappMob() {
      return `https://wa.me/77071222020`
    },
  },
}
</script>

<style lang="scss" scoped>
.room-texts {
  display: flex;
  justify-content: space-between;
  padding: 48px 16px 72px;
  max-width: 1000px;
  margin: auto;


  .info-title {
    font-size: 24px;
    margin-bottom: 24px;
    &.info-title-price {
      text-align: center;
      margin-top: 32px;
      margin-bottom: 32px;
    }
  }

  .info-des {
    font-size: 16px;
    line-height: 1.4;
    span {
      color: #ee3239;
    }
    margin-bottom: 16px;
    &--red {
      color: #ee3239;
    }
  }
  .room-info-list {
    list-style: disc inside none;
    line-height: 1.3;
  }
  .contact-buttons {
    margin-top: 48px;
    margin-left: 100px;

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
      transition: all 0.3s cubic-bezier(0.25, 0.8, 0.25, 1);

      &:hover {
        box-shadow: 0 14px 28px rgba(0, 0, 0, 0.25),
          0 10px 10px rgba(0, 0, 0, 0.22);
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
</style>
