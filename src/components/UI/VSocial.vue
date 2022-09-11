<template>
  <div class="social">
    <ul>
      <li class="social__item">
        <a href="https://www.youtube.com/channel/UCF94uYAEIOElRoIkztVq10A" target="_blank">
          <img class="social__item" src="../../assets/images/yt.svg">
        </a>
      </li>
      <li class="social__item">
        <a href="https://vk.com/tashirestate" target="_blank">
          <img class="social__item" src="../../assets/images/vk.svg">
        </a>
      </li>
      <li class="social__item">
        <a href="https://www.facebook.com/tashirestate" target="_blank">
          <img class="social__item" src="../../assets/images/fb.svg">
        </a>
      </li>
      <li class="social__item">
        <a href="https://www.instagram.com/tashirestate/" target="_blank">
          <img class="social__item" src="../../assets/images/inst.svg">
        </a>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  name: "VSocial"
}
</script>

<style scoped>
.social ul{
  flex-wrap: wrap;
  display: flex;
}
.social__item{
  margin-right: 9%;
}

</style>