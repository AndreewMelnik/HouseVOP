<template>
  <div class="background">
    <div class="wrapper">
    <div class="video__wrapper">
      <section id="video" class="video">
        <div class="row">
          <div class="">
            <a href="#" class="link_unstyled">
              <div class="video wow animate__fadeInUp">
                <img src="../assets/images/video.png" alt="" class="video__preview">
              </div>
            </a>
          </div>
        </div>
      </section>
    </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppVideo"
}
</script>

<style scoped>

.video__wrapper {
  max-width: 720px;
  margin: 0 auto;
  padding: 0 10px;

}

.video {
  position: relative;
}

.video:before {
  content: '';
  position: absolute;
  left: 0;
  top: 0;
  width: 100%;
  height: 100%;
  background-color: #242B3354;;
  opacity: .8;
  transition: all .09s ease-out;
}

.video:after {
  content: '';
  width: 100px;
  height: 100px;
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-image: url('../assets/images/play.svg');
  background-size: 100px;
  background-repeat: no-repeat;
  background-position: center;
  transition: all .09s ease-out;
}

.video:hover:before {
  opacity: 0.4;
}

.video:hover:after {
  transform: translate(-50%, -50%) scale(1.09);
}

.video__preview {
  margin: 0 auto;
}
@media (max-width: 800px) {
  .background {
    display: none;
  }
}
</style>