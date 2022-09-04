<template>
 <div class="apart">
   <div class="apart_wrapper">
     <div class="apart__card">
       <div class="apart__card-img">{{photo.title}}</div>
       <div class="apart__card-title"></div>
     </div>
   </div>
 </div>
</template>

<script>
export default {
  props: {
    photo: {
      type: Object
    }
  }
}
</script>

<style scoped>

</style>