<template>
  <div class='our-services'>
    <div class='our-services-content'>
      <div class='content-box'>
        <img src='~/assets/2.png' class='content-box-image' alt=''>
        <p class='content-box-text'>Проведение детских мероприятии со своими угощениями</p>
      </div>
      <div class='content-box'>
        <img src='~/assets/3.png' class='content-box-image' alt=''>
        <p class='content-box-text'>По доступным ценам проводим детские дни рождения</p>
      </div>
      <div class='content-box'>
        <img src='~/assets/5.png' class='content-box-image' alt=''>
        <p class='content-box-text'>Трех этажный лабиринт с винтовой горкой</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'our-services'
}
</script>

<style lang='scss' scoped>
.our-services {
  background-image: url("~/assets/fon3.png");
  background-repeat: no-repeat;
  background-position: center;
  background-size: cover;
  min-height: 550px;
  .our-services-content {
    max-width: 1000px;
    padding: 110px 24px 50px 16px;
    margin: auto;
    display: flex;
    justify-content: space-between;
    .content-box {
      width: 200px;
      display: flex;
      flex-direction: column;
      align-items: center;
      .content-box-image {
        width: 100px;
        height: 110px;
        margin-bottom: 32px;
      }
      .content-box-text {
        line-height: 1.5;
        text-align: center;
        color: white;
        font-size: 18px;
      }
    }
  }
}
</style>
