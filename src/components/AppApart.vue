<template>
 <div class="apart">
   <div class="wrapper">
     <h2 class="title" id="catalog">Наши квартиры</h2>
     <div class="apart__card-list">
       <AppApartCard
       v-for="card in cards"
       :key="card.id"
       :card_data="card"/>
     </div>
   </div>
 </div>
</template>

<script>
import AppApartCard from "@/components/AppApartCard";

export default {
  components: {AppApartCard},
  props: {},
  data() {
    return {
      cards: [
        {id: 1, title: 'Лофт — 3 этажа', image: "loft1.png"},
        {id: 2, title: 'Лофт — 2 этажа', image: "loft2.png"},
        {id: 3, title: 'Лофт — 3 этажа', image: "loft1.png"},
        {id: 4, title: 'Лофт — 2 этажа', image: "loft2.png"},
      ],
    }
  }
}

</script>

<style scoped>
.apart {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-between;
  align-items: center;
  background: #242B33;
}

.apart__card-list{
  margin-top: 100px;
  gap: 0px 30px;
  align-items: center;
  display: grid;
  grid-template-columns: 1fr 1fr;
}
.wrapper{
  max-height: 1000px;
}
@media (max-width: 700px) {
  .wrapper{
    max-height: 100%;
  }
  .apart__card-list{
    margin-top: 60px;
    gap: 30px 30px;
    grid-template-columns: 1fr;
    margin-bottom: 60px;
  }

}
</style>