<template>
  <div>
    <div class="room-info">
      <h1 class='title'>Шоу программы</h1>
      <div class="room-texts">
        <div>
          <h2 class="info-title">Квесты в залах (от 7 лет):</h2>
          <ul>
            <li>
              <p class="info-des mb-3">
                Пиратский (1 ведущий, 1ч) - Стоимость <span>17 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Bravl Stars плюс или Among US (1 ведущий, до 12 детей) - <span>28
                000тг</span> (Цена на 1,5 часа)
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Bravl Stars плюс или Among US (2 ведущих, до 15 детей) - <span>36
                000тг</span> (Цена на 1,5 часа)
              </p>
            </li>
            <li>
              <p class="info-des">
                Квесты Bravl Stars плюс или Among US + шоу фольга (1 ведущий, до
                12 детей) - <span>40 000тг</span> (Цена на 2 часа)
              </p>
            </li>
            <li>
              <p class="info-des mb-4">
                Квесты Bravl Stars плюс или Among US + шоу фольга (2 ведущих, до
                15 детей) - <span>50 000тг</span> (Цена на 2 часа)
              </p>
            </li>
          </ul>

          <h2 class="info-title">Подростковые party (от 7 лет):</h2>

          <ul>
            <li>
              <p class="info-des">
                YouTube party (1 ведущий, до 12 детей, Цена 1,5 часа) - <span>25 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                YouTube party (2 ведущих, 15- 20 детей, Цена 1,5 часа) - <span>35
                000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Tik-Tok (1 ведущий, до 12 детей, Цена 1 час) - <span>20 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Tik-Tok (2 ведущих, 15- 20 детей, Цена 1 час) - <span>28 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                YouTube party + шоу фольга (1 ведущий, до 12 детей, Цена 2 часа)
                - <span>40 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                YouTube party + шоу фольга (2 ведущих, 15- 20 детей, Цена 2
                часа) - <span>50 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Tik-Tok, Bravl Staгs или Among US + шоу фольга (1 ведущий, до 12
                детей, Цена 1,5 часа) - <span>38 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Tik-Tok, Bravl Staгs или Among US + шоу фольга (2 ведущих, 15-
                20 детей, Цена 1,5 часа) - <span>45 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                ведущий + азотное шоу с мороженым вкусное мороженное каждому
                ребенку (1 ведущий, до 12 детей, Цена 1ч 45 мин) - <span>52 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                ведущий + азотное шоу с мороженым вкусное мороженное каждому
                ребенку (2 ведущих, 15- 20 детей, Цена 1ч 45 мин) - <span>62 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пижамная вечеринка (2 ведущих (Стич и Единорог) + 1 ведьма (дух)
                15-20 детей) проектор, экран, вигвамы, бой подушками, шуточный
                спиритический сеанс - <span>48 000тг</span>
              </p>
            </li>
          </ul>
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
            <img class="contact-icon" src="~/assets/call.svg" alt="" />
            ПОЗВОНИТЬ НАМ</a
          >
        </div>
      </div>
    </div>
    <div class="room-info">
      <div class="room-texts">
        <div>
          <h2 class="info-title">Пакеты до 7 лет:</h2>
          <ul>
            <li>
              <p class="info-des">
                Пакет "Старт" (1 персонаж с программой (+ твистинг и мыльные
                пузыри), до 12 детей, время 1 час) - <span>15 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Старт" (1 персонаж с программой (+ твистинг и мыльные
                пузыри), до 12 детей, время 2 час) - <span>25 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Классический" (2 персонажа с программой (+ твистинг и
                мыльные пузыри), до 20 детей, время 1 час) - <span>20 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Классический" (2 персонажа с программой (+ твистинг и
                мыльные пузыри), до 20 детей, время 2 час) - <span>35 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Универсальный" (1 персонаж с программой (+ твистинг и
                мыльные пузыри), до 12 детей, время 2 часа (1 час аква / 1 час
                прогр.)) - <span>20 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Универсальный" (2 персонажа с программой (+ твистинг и
                мыльные пузыри), до 20 детей, время 2 часа (1 час аква / 1 час
                прогр.)) - <span>25 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Оригинальный" (персонаж с программой (+ твистинг и
                мыльные пузыри). На выбор: фольгированное шоу / поролон шоу /
                шоу гигантских мыльных пузырей, до 12 детей, время 2 часа (1 час
                аква / 1 час прогр.)) - <span>20 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Оригинальный" (2 персонажа с программой (+ твистинг и
                мыльные пузыри), до 20 детей, время 2 часа (1 час аква / 1 час
                прогр.)) - <span>25 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Азотное пати" (45 мин азотное шоу с мороженным вкусное
                мороженное каждому ребенку, 1 персонаж с программой (+ твистинг
                и мыльные пузыри) до 12 дектей, время 1 час 45 минут) - <span>50 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Азотное пати" (45 мин азотное шоу с мороженным вкусное
                мороженное каждому ребенку, 2 персонажа с программой (+ твистинг
                и мыльные пузыри) до 20 дектей, время 1 час 45 минут) - <span>55 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Под ключ" (1 персонаж, до 12 детей, время 3ч), 30мин -
                хостес: ростовая кукла или любой персонаж, 1 час до 12 детей -
                Аквагрим, 1 час анимация - персонаж с программой (+ твистинг),
                30мин (шоу на выбор) - фольгированное шоу / поролон шоу / шоу
                гигантских мыльных пузырей, круглая пиньята - с наполнением на
                10- 12 детей - <span>62 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Под ключ" (2 персонажа, до 20 детей, время 3ч), 30мин -
                хостес: ростовая кукла или любой персонаж, 1 час до 12 детей -
                Аквагрим, 1 час анимация - персонаж с программой (+ твистинг),
                30мин (шоу на выбор) - фольгированное шоу / поролон шоу / шоу
                гигантских мыльных пузырей, круглая пиньята - с наполнением на
                10- 12 детей - <span>67 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Трансформер" ( до 12-15 детей, время 1ч), 30мин -
                трансформер (Бамблби или Оптимус) с флешмобом в сопровождении
                персонажа, 30мин - персонаж (тематические игры), 1 час анимация
                - персонаж с программой (+ твистинг), 30мин (шоу на выбор) -
                фольгированное шоу / поролон шоу / шоу гигантских мыльных
                пузырей, круглая пиньята - с наполнением на 10- 12 детей - <span>30
                000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Трансформер" ( до 12-15 детей, время 1,5ч), 30мин -
                трансформер (Бамблби или Оптимус) с флешмобом в сопровождении
                персонажа, 30мин - персонаж (тематические игры), 1 час анимация
                - персонаж с программой (+ твистинг), 30мин (шоу на выбор) -
                фольгированное шоу / поролон шоу / шоу гигантских мыльных
                пузырей, круглая пиньята - с наполнением на 10- 12 детей - <span>35
                000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des">
                Пакет "Халк" ( до 12-15 детей, время 1ч), 30мин - Халк со
                флешмобом в сопровождении персонажа. Халк в сопровождении с
                персонажем, игры с тематическим материалом,дымовая пушка, 30мин
                - персонаж, 1 час анимация - персонаж с программой (+ твистинг),
                30мин (шоу на выбор) - фольгированное шоу / поролон шоу / шоу
                гигантских мыльных пузырей, круглая пиньята - с наполнением на
                10- 12 детей - <span>35 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Халк" ( до 12-15 детей, время 1,5ч), 30мин - Халк со
                флешмобом в сопровождении персонажа. Халк в сопровождении с
                персонажем, игры с тематическим материалом,дымовая пушка, 30мин
                - персонаж, 1 час анимация - персонаж с программой (+ твистинг),
                30мин (шоу на выбор) - фольгированное шоу / поролон шоу / шоу
                гигантских мыльных пузырей, круглая пиньята - с наполнением на
                10- 12 детей - <span>40 000 - 45 000тг</span>
              </p>
            </li>
            <li>
              <p class="info-des mb-3">
                Пакет "Динозавр" (до 12 - 15 детей, время 1 час). 30мин -
                Динозавр в сопровождении персонажа, 30мин - персонаж - <span>35 000тг</span>
              </p>
            </li>
          </ul>
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
            <img class="contact-icon" src="~/assets/call.svg" alt="" />
            ПОЗВОНИТЬ НАМ</a
          >
        </div>
      </div>
    </div>
    <div class="room-info">
      <div class="room-texts">
        <div>
          <h2 class="info-title">Мастер классы:</h2>
          <h2 class="info-title">Мастер класс по слаймам:</h2>
          <p class="info-des">
            Каждый участник мастер класса сможет научиться готовить слаймы
            самостоятельно.Продвинутые слаймеры также смогут узнать для себя
            новую полезную информацию по приготовлению слаймов. Во время мастер
            класса Вы узнаете о некоторых фишках и лайфхаках в приготовлении
            слаймов,о видах слаймов и об их свойствах. Море блёсток, различных
            добавок и многое другое.
          </p>
          <p class="info-des">В программе мастер класса:</p>
          <p class="info-des">
            💥Приготовление Batter slime, Milk slime, Original slime (на выбор
            ).
          </p>
          <p class="info-des">
            💵 Стоимость мастер класса: 1 800 тг/на одного человека.
          </p>
          <p class="info-des">Минимальный заказ от 10 слаймов</p>
          <p class="info-des">
            💥 Приготовление Clear slime, Fluffy slime, Cloud slime, Bubble
            slime ( на выбор)
          </p>
          <p class="info-des">
            💵 Стоимость мастер класса: 2 500 тг/на одного человека.
          </p>
          <p class="info-des mb-3">Минимальный заказ от 10 слаймов</p>

          <h2 class="info-title">Мастер класс по бейсболкам:</h2>
          <p class="info-des">
            Каждый участник мастер класса сможет научиться готовить слаймы
            самостоятельно.Продвинутые слаймеры также смогут узнать для себя
            новую полезную информацию по приготовлению слаймов. Во время мастер
            класса Вы узнаете о некоторых фишках и лайфхаках в приготовлении
            слаймов,о видах слаймов и об их свойствах. Море блёсток, различных
            добавок и многое другое.
          </p>
          <p class="info-des">
            💥Каждый участник попробует себя в роли креативного дизайнера.
          </p>
          <p class="info-des">
            💥Придумает и воплотит эксклюзивный фешн бейсболки.
          </p>
          <p class="info-des">
            💥Унесет с собой подарок ручной работы, заряженный позитивом и
            радостью и получит модную вещь и море впечатлений .
          </p>
          <p class="info-des">💵 3000 тг на ребенка, минимум 15детей</p>
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
            <img class="contact-icon" src="~/assets/call.svg" alt="" />
            ПОЗВОНИТЬ НАМ</a
          >
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import Vue from 'vue'

import 'viewerjs/dist/viewer.css'
import Viewer from 'v-viewer'
Vue.use(Viewer)

const PriceText = [
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

export default {
  name: 'prices-info',
  props: ['room'],
  computed: {
    priceInfo() {
      return PriceText
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
  }
  .info-des {
    font-size: 16px;
    line-height: 1.4;
    margin-bottom: 8px;
    span {
      color: #ee3239;
    }
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
  .mb-4 {
    margin-bottom: 24px;
  }
  .mb-3 {
    margin-bottom: 20px;
  }
  .mb-2 {
    margin-bottom: 16px;
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
ul {
  list-style-type: decimal;
}
.title {
  text-align: center;
  font-size: 36px;
  margin-top: 24px;
  margin-bottom: 16px;
}

</style>
