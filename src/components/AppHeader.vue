<template>
  <div>
    <header class="header">
      <div class="wrapper">
        <div class="header__wrapper">
          <div class="logo">
            <a href="#">
              <h1>House<span>VOP</span></h1>
              <br/>
              <h3>ЖИЛОЙ КОМПЛЕКС</h3>
            </a>
          </div>
          <nav class="navbar">
            <ul class="nav__list">
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
          </nav>
        </div>
      </div>
      <AppIntro/>
    </header>
  </div>
</template>

<script>
import AppIntro from "@/components/AppIntro";


export default {
  name: 'App',
  components: {
    AppIntro
  },

}


</script>

<style scoped>

.header {
  min-height: 100%;
  background: url(../assets/images/bg1.png) no-repeat center ;
  background-size:cover;
  position:relative;
}

header{
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  transition: all 0.2s linear;
  padding-bottom: 20px;
  z-index: 11;
}

/*.wrapper{*/
/*  padding: 0 20px;*/
/*}*/
.header__wrapper {
  display: flex;
  flex-wrap: wrap;
  align-items:flex-end;
  justify-content: space-between;
  padding-top: 5.5%;
}

.nav__list{
  display: flex;
  flex-wrap: wrap;
}

.nav__item{
  margin-right: 40px;
}
.nav__item:last-child {
  margin-right: 0;
}
a {
  color: #ffffff;
  text-decoration: none;
  font-size: 1em;
  position: relative;
  transition: all 0.6s;
}
a:before {
  content: "";
  width: 0;
  height: 0.1em;
  position: absolute;
  bottom: 0;
  left: 50%;
  background: #fff;
  transition: all 0.3s;
}
a:hover:before {
  width: 100%;
  left: 0;
  background: #fff;
}
.nav__link {
  font-family: 'Raleway';
  font-style: normal;
  font-weight: 400;
  font-size: 14px;
  line-height: 16px;
  letter-spacing: 0.05em;
}

.nav__link:hover, .nav__link:focus, .nav__link:active {
  /*opacity: 0.75;*/
  /*transition: 1s;*/
}
@media (max-width: 800px) {
  .navbar {
    display:none
  }
}
</style>