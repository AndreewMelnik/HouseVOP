  <template>
    <div class="footer__background">
      <div class="wrapper">
      <footer class="footer" id="signin">
          <div class="logo"><a href="#">
              <h1>House<span>VOP</span></h1>
              <br/>
              <h3>ЖИЛОЙ КОМПЛЕКС</h3></a>
          </div>
          <VMenu class="footer__item"/>
          <VMenu class="footer__item"/>
          <div class="contacts footer__item">
            <ul>
              <li class="contacts__item">Адрес: Наб. реки Фонтанки 10-15</li>
              <li class="contacts__item">Телефон: 8 (812) 123-45-67</li>
              <li class="contacts__item">Отдел продаж: 10:00 - 20:00</li>
              <li class="contacts__item">E-mail: <mark>vip@housevip.ru</mark></li>
            </ul>
            <VSocial/>
          </div>
      </footer>
      </div>
    </div>
  </template>

<script>
import VMenu from "@/components/UI/VMenu";
import VSocial from "@/components/UI/VSocial";

export default {
  name: "AppFooter",
  components: {VSocial, VMenu}
}
</script>

<style scoped>
.footer__background{
  background-color: #2D343C;
}
.footer{
  display: grid;
  grid-template-columns: repeat(4,1fr);
  padding-top: 60px;
  gap: 47px;
  padding-bottom: 50px;
}
.contacts li{
  margin-bottom: 15px;
}

.contacts mark {
  background-color: transparent;
  color: rgba(212, 193, 127, 1);
  font-weight: 700;
}

.contacts__item{
  font-family: 'Raleway';
  font-size: 14px;
  line-height: 16px;
  letter-spacing: 0.05em;
  color: #FFFFFF;
}

@media (max-width: 800px) {
  .wrapper{
    width:90%;
    padding: 0px;
  }
  .footer__item:nth-child(2){
    display: none;
    position: absolute;
  }
  .footer {
    grid-template-columns: repeat(3, 1fr);
    gap: 30px;

  }
  .logo{
    font-size: 13.5px;
  }
  .logo h3 {
    font-size: 10px;
    line-height: 12px;
  }
  .contacts__item{
    font-size: 12px;
    line-height: 14px;
  }
  .contacts li{
    margin-bottom: 10px;
  }
}
@media (max-width: 480px) {

  .contacts__item{
    font-size: 9px;
    line-height: 10px;
  }
  .contacts li{
    margin-bottom: 5px;
}}



</style>