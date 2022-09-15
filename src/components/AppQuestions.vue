<template>
  <div class="background">
    <div class="wrapper">
      <h1 class="title">Есть вопросы?</h1>
      <form action="#" method="POST">
        <div class="form">
          <div class="form__item ">
            <span class="form__item-text">*Мы никому не передаем ваши данные. И не сохраняем ваш номер в базу.</span>
          </div>
          <div class="form__item">
            <input type="text" class="form-control" placeholder="Ваше имя">
          </div>
          <div class="form__item">
            <input type="text" class="form-control" placeholder="Ваш телефон">
          </div>
          <div class="form__item">
            <button class="btn btn-accent">Посмотреть район</button>
          </div>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
export default {
  name: "AppQuestions"
}
</script>

<style scoped>

.form {
  padding-top: 50px;
  display: flex;
}

.form__item-text {
  font-family: 'Raleway';
  font-style: normal;
  font-weight: 400;
  font-size: 13px;
  line-height: 16px;
  text-align: center;
}

.form__item {
  width: calc(50% - 15px);
  margin-bottom: 180px;
  margin-right: 30px;
}

.form-control {
  width: 85%;
  border: none;
  background-color: rgba(255, 255, 255, .2);
  transition: all .09s ease-out;
  padding: 16px;
  color: #fff;
  text-align: center;
}

.form-control:focus {
  outline: none;
  background-color: rgba(255, 255, 255, .24);
}
@media (max-width:800px) {
  .wrapper {
    display: flex;
    flex-wrap: wrap;
    padding-bottom: 20%;
  }
  form{
    margin: 0 auto;
  }
  .form {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap:20% 5%;
    padding-top: 20%;
    margin-left: 0px;
  }
  .form__item {
    width: 100%;
    margin-bottom: 0px;
    margin-right: 0px;
  }
  .form__item:nth-child(1){
    display: none;
    position: absolute;
  }
  .form__item:nth-child(4){
    /*padding-left: 80px;*/
    /*margin: 0 auto;*/
  }

  .title {
    padding-top: 10px;
    max-width: 100%;
  }
  .form__title p {
    width:100%;
    text-align: center;
    font-size: 14px;
    padding-top: 10%;
  }
  .form-control {
    padding: 16px 6px 16px 6px;
  }
}
@media (max-width:480px) {
  .form__item-text {
    font-size: 11px;
  }
  .btn{
    width:93%
  }
  .form {
    padding-top: 10%;
  }
  .title {
    padding-top: 20%;
  }
}




</style>