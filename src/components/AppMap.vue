<template>
  <div class="background">
    <div class="wrapper">
      <div class="map" id="locations">
        <h2 class="title">Район на карте</h2>
        <iframe
            src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d1998.2444236685037!2d30.337639216097188!3d59.94467898187832!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x4696317353b89bb9%3A0x4a5baf20e1544c1b!2z0L3QsNCx0LXRgNC10LbQvdCw0Y8g0YDQtdC60Lgg0KTQvtC90YLQsNC90LrQuCwgMTAsINCh0LDQvdC60YIt0J_QtdGC0LXRgNCx0YPRgNCzLCDQoNC-0YHRgdC40Y8sIDE5MTE4Nw!5e0!3m2!1sru!2sua!4v1599295496038!5m2!1sru!2sua"
            width="1110" height="358" style="border:0;" allowfullscreen="" aria-hidden="false" tabindex="0"
            title="our adress on map">
          >
        </iframe>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  name: 'AppMap',
}
</script>
<style scoped>
.map iframe{
  padding-top: 100px;
}
@media (max-width: 1200px) {
  iframe {
    width: 100%;
  }
  .map iframe{
    padding-top: 8%;
  }
}

@media (max-width: 414px) {
  iframe {
    height: 250px;
  }
}
</style>


