<template>
  <section class="app-form">
    <div class="wrapper">
      <div class="title">
        <h2>Хотите посмотреть?</h2>
        <div class="form__title"><p>Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem
          Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный
          печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. </p>
        </div>
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

.form__title p {
  font-family: 'Raleway';
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  padding-top: 50px;
  width: 535px;
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
  width: 220px;
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
</style>