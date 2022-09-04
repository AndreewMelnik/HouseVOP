<template>
<div class="info">
  <div class="info__cards">
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/park.svg">
      <h2 class="info__card-title">Рядом исторические парки и скверы</h2>
    </div>
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/building.svg">
      <h2 class="info__card-title">Полностью обустроенный</h2>
    </div>
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/fountain.svg">
      <h2 class="info__card-title">10 фонтанов на территории</h2>
    </div>
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/velo.svg">
      <h2 class="info__card-title">6 км <br/>велодорожек</h2>
    </div>
<!--    <span class="rome">II</span>-->
  </div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>
.info{
  background:#242B33;
}
.info__cards{
  display: flex;
  justify-content: center;
  padding-top: 194px;
}
.info__card{
  display: flex;
  flex-direction: column;
  align-self: last baseline;
  margin-right: 25px;
}
.info__card-img{
  max-width: 80px;
  margin: 0 auto;
}

.info__card-title{
  max-width: 200px;
  font-family: 'Raleway';
  font-weight: 300;
  font-size: 19px;
  line-height: 27px;
  text-align: center;
  margin-top: 50px;
}
/*.rome{*/
/*  position: absolute;*/
/*  left: 74%;*/
/*  top: 100%;*/
/*  font-family: 'Playfair Display';*/
/*  font-size: 400px;*/
/*  opacity: 0.02;*/
/*}*/
</style>