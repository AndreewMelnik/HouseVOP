<template>
  <ul class="menu__list">
    <li>
      <router-link
          class="menu__list-link"
          to="/about"
      >
        О комплексе
      </router-link>
    </li>
    <li>
      <router-link
          class="menu__list-link"
          to="/location"
      >
        Район
      </router-link>
    </li>
    <li>
      <router-link
          class="menu__list-link"
          to="/catalog"
      >
        Каталог квартир
      </router-link>
    </li>
    <li>
      <router-link
          class="menu__list-link"
          to="/mortgage"
      >
        Ипотека
      </router-link>
    </li>
    <li>
      <router-link
          class="menu__list-link"
          to="/contacts"
      >
        Контакты
      </router-link>
    </li>
  </ul>
</template>
<script>
export default {
  name: 'v-menu',
}
</script>
<style scoped>

.menu__list-link {
  color: #fff;
  font-family: 'Raleway';
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  letter-spacing: 0.05em;
}
.menu__list li{
  margin-bottom: 15px;
}

@media (max-width: 800px) {
  .menu__list-link {
    font-size: 12px;
    line-height: 12px;
  }
  .menu__list li{
    margin-bottom: 10px;
  }
@media (max-width: 480px) {
  .menu__list-link {
    font-size: 9px;
    line-height: 10px;
  }
  .menu__list li{
    margin-bottom: 5px;
  }
}
}
</style>