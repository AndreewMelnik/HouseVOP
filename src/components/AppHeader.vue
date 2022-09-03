<template>
  <div>
    <header class= "header" >
      <div class="wrapper">
        <div class="header__wrapper">
          <div class="logo">
            <a href="#">
              <h1>House<span>VOP</span></h1>
              <br/>
              <h2>ЖИЛОЙ КОМПЛЕКС</h2>
            </a>
          </div>
          <nav class="navbar">
            <ul class="nav__list">
              <li class="nav__item">
                <a class="nav__link" href="#articles">О комплексе</a>
              </li>
              <li class="nav__item">
                <a class="nav__link" href="#locations">Район</a>
              </li>
              <li class="nav__item">
                <a class="nav__link" href="#locations">Каталог квартир</a>
              </li>
              <li class="nav__item">
                <a class="nav__link" href="#videos">Ипотека</a>
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
  }
}


</script>

<style scoped>

.header {
  min-height: 100vh;
  background: url(../assets/images/Rectangle.png) no-repeat center ;
  background-size:cover;
  position:relative;
}

.logo{
font-family: 'Post No Bills Jaffna SemiBold Regular',serif;
font-size: 17.5px;
line-height: 0.5;
}
.logo h2{
  font-family: 'Raleway';
  font-size: 12px;
  line-height: 14px;
  letter-spacing: 0.12em;
  margin-top: 5px;
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
</style>