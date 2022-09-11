<template>
<div class="intro">
  <div class="wrapper">
  <div class="intro__wrapper">
    <div class="intro__title">Жилой комплекс <br/>в историческом центре</div>
    <a class="intro__logo" href="#articles">
<!--      <img class="intro__logo-img" src="../assets/images/mouse.svg" alt="mouse" />-->
    </a>
    <div class="intro__contacts">
        <div class="intro__contacts-caption">
          <div class="intro__contacts-geo"></div>
          <span class="intro__contacts-title">Наб. реки Фонтанки 10-15</span>
        </div>
        <div class="intro__contacts-caption">
          <div class="intro__contacts-tel"></div>
          <h3 class="intro__contacts-title">8 (812) 123-45-67</h3>
        </div>
    </div>
  </div>
  </div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.intro{
  margin-top: 225px
;
}
.intro__wrapper{
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;

}
.intro__title{
  font-family: 'Playfair Display';
  font-size: 48px;
  line-height: 64px;
  text-align: center;
  color: #D4C17F;
}
.intro__logo{
  margin-top: 100px;
  display: inline-block;
  padding-bottom: 40px;
  background: url("../assets/images/mouse.svg") no-repeat 95% center;
  transition: all 0.2s;
  width: 40px;
  height: 40px;
}

.intro__logo:hover, .intro__logo:focus {
  background: url("../assets/images/mouse.svg") no-repeat bottom center;
}
.intro__contacts{
  display: flex;
  flex-wrap: wrap;
  margin-top: 160px;
  width: 62%;
  justify-content: space-around;
}
.intro__contacts-caption{
  display: flex;
  margin-top: 2%;
}
.intro__contacts-title{
  font-family: 'Raleway';
  font-size: 17px;
  line-height: 21px;
}
.intro__contacts-geo{
  background: url(../assets/images/geo.svg) no-repeat right;
  background-size: 14px;
  width: 15px;
  height: 21px;
  margin-right: 18px;

}
.intro__contacts-tel{
  background: url(../assets/images/tel.svg) no-repeat right;
  background-size: 14px;
  width: 15px;
  height: 21px;
  margin-right: 18px;
}

@media (max-width: 800px) {
  .intro__title{
    font-size: 37px;
  }
  .intro__contacts-title{
    font-size: 15px;
  }
}
@media (max-width: 480px) {
  .intro__contacts-title{
    font-size: 13px;
  }
}

</style>