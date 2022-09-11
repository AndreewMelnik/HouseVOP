<template>
<div class="background">
  <div class="wrapper">
  <div class="info__cards" id="articles">
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/park.svg">
      <h3 class="info__card-title">Рядом исторические парки и скверы</h3>
    </div>
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/building.svg">
      <h3 class="info__card-title">Полностью обустроенный</h3>
    </div>
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/fountain.svg">
      <h3 class="info__card-title">10 фонтанов на территории</h3>
    </div>
    <div class="info__card">
      <img class="info__card-img" src="../assets/images/velo.svg">
      <h3 class="info__card-title">6 км <br/>велодорожек</h3>
    </div>
<!--    <span class="rome">II</span>-->
  </div>
</div>
</div>
</template>

<script>
export default {

}
</script>

<style scoped>

.info__cards{
  display: flex;
  justify-content: center;
  padding-top: 194px;
}
.info__card{
  display: flex;
  flex-direction: column;
  align-self: last baseline;
  margin-right: 2%;
}
.info__card-img{
  max-width: 80px;
  margin: 0 auto;
}

.info__card-title {
  max-width: 200px;
  font-family: 'Raleway';
  font-weight: 300;
  font-size: 19px;
  line-height: 27px;
  text-align: center;
  margin-top: 50px;
}

@media (max-width: 1200px) {
  .info__card-title {
    font-size: 17px;
  }

  .info__card {
    margin-right: 1.5%;
  }
}

@media (max-width: 800px) {
  .info__cards {
    display: grid;
    justify-content: center;
    grid-template-columns: 1fr 1fr;
    gap:60px;
  }

  .info__card {
    align-items: center;
  }
}

@media (max-width: 480px) {
  /*  .info__cards {*/
  /*  }*/
  /*}*/
  .info__card-title {
    font-size: 14px;
  }
}



</style>
