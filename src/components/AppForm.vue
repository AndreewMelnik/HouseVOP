<template>
  <section class="app-form">
    <div class="wrapper">
      <div class="form__title">
          <h2>Хотите посмотреть?</h2>
          <p>Lorem Ipsum - это текст-"рыба", часто используемый в печати и вэб-дизайне. Lorem Ipsum является стандартной "рыбой" для текстов на латинице с начала XVI века. В то время некий безымянный печатник создал большую коллекцию размеров и форм шрифтов, используя Lorem Ipsum для распечатки образцов. </p>
      </div>

          <form action="#" method="POST">
            <div class="form">
              <div class="form__item">
                <input type="text" class="form-control" placeholder="Ваше имя">
              </div>

              <div class="form__item">
                <input type="text" class="form-control" placeholder="Ваш телефон">
              </div>

              <div class="form__item mb-0 d-none d-lg-block">
                <span class="form__item-text">*Мы никому не передаем ваши данные. И не сохраняем ваш номер в базу.</span>
              </div>

              <div class="form__item mb-0 mt-2 mt-lg-0">
                <button class="btn btn-accent">Посмотреть район</button>
                <div class="d-lg-none d-block mt-2">
                </div>
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
.app-form{
  background: url(../assets/images/bg2.png) no-repeat center ;
  background-size:cover;
  position:relative;
  height:560px


}
.form__title h2{
  padding-top: 180px;
}
.form__title p{
  font-family: 'Raleway';
  font-weight: 400;
  font-size: 16px;
  line-height: 24px;
  padding-top: 50px;
  max-width: 535px;
}
.form{
  padding-top: 265px;
}
.form__item-text{
  font-family: 'Raleway';
  font-style: normal;
  font-weight: 400;
  font-size: 13px;
  line-height: 16px;

  /* or 123% */
  text-align: center;
}

.form {
  display: flex;
  flex-flow: row wrap;
  justify-content: space-between;
  width: 100%;
}

.form__item {
  width: calc( 50% - 15px );
  margin-bottom: 35px;
}
.form-control {
  width: 100%;
  border: none;
  background-color: rgba(255, 255, 255, .2);
  transition: all .09s ease-out;
  padding: 13px;
  color: #fff;
}

.form-control:focus {
  outline: none;
  background-color: rgba(255, 255, 255, .24);
}
.wrapper{
  display: flex;
}
</style>