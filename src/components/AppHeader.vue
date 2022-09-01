<template>
  <div>
    <header class= "header" >
      <div class="wrapper">
        <div class="header__wrapper">
          <div class="logo">
            <a href="#">
              <h1>House<span>vop</span></h1>
            </a>
          </div>
          </div>
          <nav class="navbar">
            <ul class="nav__list">
              <li class="nav__item">
                <a class="nav__link" href="#articles">О комплексе</a>
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
    </header>
  </div>
</template>

<script>
export default {

  data() {
    return {

    }
  },
}
</script>

<style scoped>
@font-face {
  font-family: 'Post No Bills Jaffna SemiBold Regular';
  font-style: normal;
  font-weight: normal;
  src: local('Post No Bills Jaffna SemiBold Regular'), url('../assets/fonts/PostNoBillsJaffna-SemiBold.woff') format('woff');
}
.header {
  min-height: 100vh;
  background: url(../assets/images/Rectangle.png) no-repeat center ;
  background-size:cover;
  position:relative;
}

.logo{
font-family: 'Post No Bills Jaffna SemiBold Regular',serif;
font-weight: 600;
font-size: 27px;
line-height: 0.5;
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

.navbar{
}

.nav__list{
  display: flex;
  flex-wrap: wrap;
}

.nav__item{
  margin-right: 82px;
}
.nav__item:last-child {
  margin-right: 0;
}

.nav__link{
font-family: 'Raleway';
font-style: normal;
font-weight: 400;
font-size: 14px;
line-height: 16px;
letter-spacing: 0.05em;
}

.nav__link:hover, .nav__link:focus, .nav__link:active {
  opacity: 0.75;
  transition: 1s;
}
</style>