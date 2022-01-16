<template>
  <div class="footer">
    <div class="footer-content">
      <div class="info">
        <h2 class='title'>КОНТАКТЫ</h2>
        <h2 class='title-address'>ЗАЛЫ #1 и #2:</h2>
        <h2 class='address'>Алматы, микрорайон Мамыр-1, 29</h2>
        <h2 class='title-address'>ЗАЛ #3:</h2>
        <h2 class='address'>Алматы, микрорайон Мамыр-1, 29/6</h2>
        <a class='tel-number' href='tel: +7(727)2295509'>+7(727) 229 55 09</a>
        <a class='tel-number' href='tel: +7(707)1222020'>+7(707) 122 20 20</a>
      </div>
      <div class="extra-info">
        <img src='~/assets/15.png' class='footer-map' alt=''>
      </div>
      <div class='contact-buttons'>
        <a class='contact-button whatsapp whatsapp-des' :href='whatsapp' target='_blank'> <img class='contact-icon' src='~/assets/whatsapp.svg' alt=''> НАПИСАТЬ НАМ В WHATSAPP</a>
        <a class='contact-button whatsapp whatsapp-mob' :href='whatsappMob' target='_blank'> <img class='contact-icon' src='~/assets/whatsapp.svg' alt=''> НАПИСАТЬ НАМ В WHATSAPP</a>
        <a class='contact-button' href='tel: +7(707)1222020' target='_blank'> <img class='contact-icon' src='~/assets/call.svg' alt=''> ПОЗВОНИТЬ НАМ</a>
      </div>
    </div>
    <div class='footer-underline'>
      <img class='footer-logo' src='~/assets/1.png' alt=''>
      <img src='~/assets/14.png' class='footer-kids' alt=''>
    </div>
    <div class='footer-soc'>
      <div class='soc-icons'>
        <a href='https://www.facebook.com/bam.bino.7547' target='_blank'><img src='~/assets/16.png' class='soc-icon' alt=''></a>
        <a href='https://www.instagram.com/bambino.kz/' target='_blank'><img src='~/assets/17.png' class='soc-icon' alt=''></a>
        <a href='https://vk.com/id404636997' target='_blank'><img src='~/assets/18.png' class='soc-icon' alt=''></a>
      </div>

    </div>
  </div>
</template>

<script>
export default {
  name: 'footer-component',
  computed: {
    whatsapp() {
      return  `https://web.whatsapp.com/send?phone=77071222020&text=Добрый день`
    },
    whatsappMob(){
      return `https://wa.me/77071222020?text=Добрый день`
    }
  }
}
</script>

<style lang="scss" scoped>
.footer {
  background-image: url('~/assets/ceni_fon2.png');
  background-repeat: no-repeat;
  background-size: cover;
  background-position: center;
  min-height: 300px;
  .footer-content {
    max-width: 1000px;
    padding: 50px 24px 50px 16px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    align-items: center;
    position: relative;
.contact-buttons {
  position: absolute;
  right: 0;
  left: 0;
  bottom: 60px;
  margin: auto;
  .contact-button {
    margin: auto auto 16px auto;
    text-decoration: none;
    padding: 12px 24px;
    color: white;
    background: rgba(238,50,57,1);
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
    .info {
      h2 {
        font-size: 22px;
        color: white;
        &.title {
          margin-bottom: 28px;
        }
        &.address {
          margin-bottom: 20px;
        }
      }
      .tel-number {
        text-decoration: none;
        color: white;
        display: block;
        margin-bottom: 12px;
      }
    }
  }
  .footer-underline {
    height: 40px;
    background: rgba(238,50,57,1);
    position: relative;
    .footer-logo {
      position: absolute;
      right: 0;
      left: 0;
      bottom: -5px;
      margin: auto;
      width: 120px;
      height: auto;
    }
    .footer-kids {
      position: absolute;
      right: 100px;
      left: auto;
      bottom: -25px;
      margin: auto auto auto auto ;
      width: 220px;
      height: auto;
    }
  }
  .footer-soc {
    background: white;
    min-height: 50px;
    padding: 32px 0 24px 0;
    .soc-icons {
      display: grid;
      grid-template-columns: auto auto auto;
      justify-items: center;
      justify-content: center;
      gap: 12px;
      .soc-icon {
        width: 50px;
      }
    }
  }
  .footer-map {
    width: 400px;
    height: auto;
  }
}
</style>
