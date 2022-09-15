<template>
  <div class="mobile-menu-wrapper">
    <input id="menu-toggle" type="checkbox" />
    <label class='menu-button-container' for="menu-toggle">
      <div class='menu-button' ></div>
    </label>
    <ul class="mobile-menu" ref="mobile-menu">
      <li class="nav__item">
        <a class="nav__link" href="#articles">О комплексе</a>
      </li>
      <li class="nav__item">
        <a class="nav__link" href="#catalog">Каталог квартир</a>
      </li>
      <li class="nav__item">
        <a class="nav__link" href="#form">Ипотека</a>
      </li>
      <li class="nav__item">
        <a class="nav__link" href="#locations">Район</a>
      </li>
      <li class="nav__item">
        <a class="nav__link" href="#signin">Контакты</a>
      </li>
    </ul>
  </div>

</template>
<script>
export default {
  name: 'VMobile-Menu'
}

</script>

<style scoped>

.mobile-menu {
  position: absolute;
  top: 0;
  right: 0;
  left: 0;
  background-color: #242B33;
  flex-direction: column;
  height: 0;
  opacity: 0;
  transition: all 0.4s ease;
}
.mobile-menu {
  font-size: 0;
  transition: all 0.4s ease;
}

.active-menu {
  padding: 10px;
  font-size: 18px;
}
.menu-button-container {
  display: none;
  height: 100%;
  width: 30px;
  cursor: pointer;
  flex-direction: column;
  justify-content: center;
  align-items: center;
}
#menu-toggle {
  display: none;
}
.menu-button, .menu-button::before, .menu-button::after {
  display: block;
  background-color: #fff;
  position: absolute;
  height: 4px;
  width: 30px;
  transition: transform 400ms cubic-bezier(0.23, 1, 0.32, 1);
  border-radius: 1px;
  z-index: 100;
}
.menu-button::before {
  content: '';
  margin-top: -8px;
}
.menu-button::after {
  content: '';
  margin-top: 8px;
}
#menu-toggle:checked + .menu-button-container .menu-button::before {
  margin-top: 0px;
  transform: rotate(405deg);
}
#menu-toggle:checked + .menu-button-container .menu-button {
  background: rgba(255, 255, 255, 0);
}
#menu-toggle:checked + .menu-button-container .menu-button::after {
  margin-top: 0px;
  transform: rotate(-405deg);
}
@media (max-width: 800px) {
  .menu-button-container {
    display: flex;
    margin-left: auto;
    margin-top: 50%;
  }
}
</style>