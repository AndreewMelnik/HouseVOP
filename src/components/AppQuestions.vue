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

</style>