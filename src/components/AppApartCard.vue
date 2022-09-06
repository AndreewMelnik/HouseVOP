<template>
   <div class="cards__card">

         <div class="room wow animate__fadeInUp" data-wow-delay=".2s" data-wow-offset="200">
           <img :src=' require("../assets/images/" + card_data.image)' alt="" class="card__photo">
           <h3 class="card__title">{{card_data.title}}</h3>
         </div>

 </div>
</template>

<script>
export default {
  name:"AppApartCard",
  props: {
    card_data: {
      type:Object,
      default() {
        return {}
      }
    }
  },
  data() {
    return {

    }
  },
}

</script>

<style scoped>
.cards__card{
  color:white;
}
.cards__card img{
   /*width: 100%;*/
  margin: 30px 0;
  transition: 0.5s;
 }
.card__title{
  position: relative;
  top: -100px;
  left: 50px;
  font-family: 'Raleway';
  font-weight: 400;
  font-size: 24px;
}
.cards__card:hover .cards__card img{
  transform: scale(1.1);
}

</style>