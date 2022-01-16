<template>
  <div>
    <div class="header">
      <div class="header-content">
        <nuxt-link to="/">
          <img src="~/assets/logo.png" alt="logo" class="logo" />
        </nuxt-link>
        <div class="header-contacts">
          <div class="header-soc">
            <a href='https://www.instagram.com/bambino.kz/' target='_blank' class='header-soc-icon-link'>
              <img class='header-soc-icon' src='~/assets/instagram-header.svg' alt=''>
            </a>
            <a :href='whatsapp' target='_blank' class='header-soc-icon-link whatsapp-des'>
              <img class='header-soc-icon' src='~/assets/wa-header.svg' alt=''>
            </a>
            <a :href='whatsappMob' target='_blank' class='header-soc-icon-link whatsapp-mob'>
              <img class='header-soc-icon' src='~/assets/wa-header.svg' alt=''>
            </a>
          </div>
          <p class='header-contacts-address'>ЖК Спутник, <br>мкр. Мамыр 1, 29/6</p>
          <a class='header-contacts-phone' href='tel: +77071222020' target='_blank'>+7 707 122 20 20</a>
        </div>
      </div>
      <div class='header-content-sec'>
        <ul class='header-links'>
          <li><nuxt-link to='/contacts'>НАШИ ЗАЛЫ</nuxt-link></li>
          <li><nuxt-link to='/price'>ЦЕНЫ</nuxt-link></li>
          <li><nuxt-link to='/gallery'>ГАЛЕРЕЯ</nuxt-link></li>
          <li><nuxt-link to='/'>КВЕСТЫ</nuxt-link></li>
          <li><nuxt-link to='/contacts'>КОНТАКТЫ</nuxt-link></li>
        </ul>
        <div class='header-main-image-box'>
          <img class='header-main-image' src='~/assets/head.png' alt=''>
        </div>
        <div class='header-title-text' />
      </div>

    </div>
    <div class='header-content-info'>
      <div class='header-info'>
        <div>
          <p>«Центр семейного отдыха клуб «Bаmbino» приглашает провести посиделку с друзьями или праздник Вашей мечты в оригинальном стиле!</p>
          <p class='red'>У нас захватывающие лабиринты, квест комнаты, профессиональное караоке, шоу программы для детей любого возраста.</p>
          <p>Залы оборудованы кухнями с сервировкой на 22 человек, очень удобно принести угощение с собой или заказать доставку прямо к праздничному столу. Подарите ребенку сказку и яркие впечатления на весь год»</p>
        </div>
        <div class='contact-buttons'>
          <a class='contact-button whatsapp whatsapp-des' :href='whatsapp' target='_blank'> <img class='contact-icon' src='~/assets/whatsapp.svg' alt=''> НАПИСАТЬ НАМ В WHATSAPP</a>
          <a class='contact-button whatsapp whatsapp-mob' :href='whatsappMob' target='_blank'> <img class='contact-icon' src='~/assets/whatsapp.svg' alt=''> НАПИСАТЬ НАМ В WHATSAPP</a>
          <a class='contact-button' href='tel: +7(707)1222020' target='_blank'> <img class='contact-icon' src='~/assets/call.svg' alt=''> ПОЗВОНИТЬ НАМ</a>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'main-page',
  computed: {
    whatsapp() {
      return  `https://web.whatsapp.com/send?phone=77071222020`
    },
    whatsappMob(){
      return `https://wa.me/77071222020`
    }
  }
}
</script>

<style lang="scss" scoped>

.header-content-info {
  background-color: #cddaed;
  background-image: url("~/assets/1.png");
  background-repeat: no-repeat;
  background-size: 350px;
  background-position: 105% 107%;
  min-height: 560px;
  .header-info {
    max-width: 1000px;
    padding: 110px 24px 50px 16px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    p {
      font-size: 18px;
      margin-bottom: 24px;
      &.red {
        color: rgba(238, 50, 57, 1);
      }
    }
    .contact-buttons {

      margin: auto;
      .contact-button {
        margin: auto auto 16px 32px;
        text-decoration: none;
        padding: 12px 24px;
        color: white;
        background: #27557a;
        border-radius: 20px;
        display: flex;
        align-items: center;
        width: 215px;
        box-shadow: 0 3px 6px rgba(0,0,0,0.16), 0 3px 6px rgba(0,0,0,0.23);
        transition: all 0.3s cubic-bezier(.25,.8,.25,1);
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
}
.header {
  background: rgb(13, 121, 177);
  background: linear-gradient(
    132deg,
    rgba(13, 121, 177, 1) 8%,
    rgba(206, 60, 74, 1) 77%,
    rgba(238, 50, 57, 1) 100%
  );
  min-height: 700px;
  .header-content {
    max-width: 1000px;
    padding: 16px 24px 50px 16px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: flex-start;

    .logo {
      width: 200px;
      height: auto;
    }

    .header-contacts {
      .header-soc {
        .header-soc-icon-link {
          &:first-child {
            margin-right: 8px;
          }
        }
        .header-soc-icon {
          width: 38px;
          height: 38px;

        }
      }
      .header-contacts-address {
        color: white;
        margin: 12px 0;
        font-size: 22px;
      }
      .header-contacts-phone {
        text-decoration: none;
        color: #275579;
        font-size: 22px;
      }
    }

  }
  .header-content-sec {
    position: relative;
    .header-main-image-box {
      position: absolute;
      top: 40px;
      left: 0;
      right: 0;
      max-width: 1000px;
      margin: auto;

      .header-main-image {
        width: 100%;
        height: 500px;

      }
    }
    .header-title-text {
      position: absolute;
      top: 452px;
      left: 0;
      right: 0;
      margin: auto;
      transform: skew(
          -35deg);
      background-color: #ee3239;
      width: 412px;
      height: 80px;
      &:after {
        content: 'ДЕТСКИЕ ИГРОВЫЕ КОМНАТЫ И КВЕСТЫ';
        position: absolute;
        top: 14px;
        left: 0;
        bottom: 0;
        right: 0;
        color: white;
        font-size: 28px;
        margin: auto;
        transform: skew(
            35deg);
        text-align: center;
      }
    }

    .header-links {
      max-width: 700px;
      margin: auto;
      text-decoration: none;
      display: flex;
      gap: 24px;
      justify-content: space-around;
      li {
        background-color: rgba(238, 50, 57, 1);
        height: 50px;
        padding: 12px 8px;
        width: 100px;
        text-align: center;
        border-radius: 50% / 10%;
        box-shadow: 0 19px 38px rgba(0,0,0,0.30), 0 15px 12px rgba(0,0,0,0.22);
      }
      a {
        text-decoration: none;
        font-weight: 500;
        color: white;

      }
    }
  }

}

.whatsapp-des {
  @media screen and (max-width: 1000px) {
    display: none;
  }
}

.whatsapp-mob {
  @media screen and (min-width: 1000px) {
    display: none;
  }
}
</style>
