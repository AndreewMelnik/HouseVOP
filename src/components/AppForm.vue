<template>
  <section class="app-form" id="form">
    <div class="wrapper">
      <div class="title">
        <h2>Хотите посмотреть?</h2>
        <h3 class="form__title"><p>Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem
          Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный
          печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. </p>
        </h3>
      </div>

      <form action="#" method="POST">
        <div class="form">
          <div class="form__item">
            <input type="text" class="form-control" placeholder="Ваше имя">
          </div>

          <div class="form__item">
            <input type="text" class="form-control" placeholder="Ваш телефон">
          </div>

          <div class="form__item ">
            <span class="form__item-text">*Мы никому не передаем ваши данные. И не сохраняем ваш номер в базу.</span>
          </div>

          <div class="form__item">
            <button class="btn btn-accent">Посмотреть район</button>
          </div>
        </div>
      </form>
    </div>
  </section>
</template>

<script>
export default {
  name: "AppForm"
}
</script>

<style scoped>
.app-form {
  background: url(../assets/images/bg2.png) no-repeat center;
  background-size: cover;
  position: relative;
  height: 560px
}

.title{
  padding-top: 180px;
  max-width: 50%;
}

.form__title p {
  font-family: 'Raleway';
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  padding-top: 50px;
  width: 87%;
}

.form {
  padding-top: 265px;
}

.form__item-text {
  font-family: 'Raleway';
  font-style: normal;
  font-weight: 400;
  font-size: 13px;
  line-height: 16px;
  text-align: center;
}

.form {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  /*width: 100%;*/
  margin-left: 35px;
}

.form__item {
  width: calc(50% - 15px);
  margin-bottom: 35px;
}

.form-control {
  width: 85%;
  border: none;
  background-color: rgba(255, 255, 255, .2);
  transition: all .09s ease-out;
  padding: 13px;
  color: #fff;
  text-align: center;
}

.form-control:focus {
  outline: none;
  background-color: rgba(255, 255, 255, .24);
}

.wrapper {
  display: flex;

}

@media (max-width:1200px) {
  .form-control {
    width: 83%;
    font-size:13px;
  }
}
@media (max-width:800px) {
  .form {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap:20%;
    padding-top: 20%;
    margin-left: 0px;
  }
  .form__item {
    width: 100%;
    margin-bottom: 0px;
  }
  .title {
    padding-top: 10px;
    max-width: 100%
  ;
  }
  .app-form {
    height: 100%
  }
  .wrapper {
    display: flex;
    flex-wrap: wrap;
    padding-bottom: 10%;
  }
  .form__title p {
    width:100%;
    text-align: center;
    font-size: 14px;
    padding-top: 10%;
  }
}
@media (max-width:480px) {
  .form__item-text {
    font-size: 11px;
  }
}
</style>