<template>
  <div>
    <div class="on_footer">
      <div class="footer-logo">
        <img src="images/Spodaryk_Logo.png" alt="logo">
      </div>
      <div class="footer-title">
        Замовте свій унікальний набір посуду
      </div>
      <div class="footer-contacts">
        <a href="tel:+38 097 656 01 57">+38 097 656 01 57</a>
        <a href="mailto:spodarykgroup@gmail.com">spodarykgroup@gmail.com</a>
      </div>
      <ul class="links">
        <li>
          <v-btn icon large href="https://www.instagram.com/spodaryk.group/" target="_blank">
            <icon-insta />
          </v-btn>
        </li>
        <li>
          <v-btn icon large small href="https://www.facebook.com/spodaryk.group" target="_blank">
            <icon-facebook />
          </v-btn>
        </li>
        <li>
          <v-btn icon large link href="mailto:spodarykgroup@gmail.com" target="_blank">
            <icon-gmail />
          </v-btn>
        </li>
      </ul>
    </div>
    <footer id="footer-animation">
      Всі фото і відео матеріали належать Spodaryk Group (ФОП Сподарик М.) та їх
      <br>
      власникам і не можуть бути використані без погодження з власниками.
      <br>
      © Made by Yurii Oleksovskyi, 2021
    </footer>
  </div>
</template>

<script>
import IconGmail from '~/components/icons/icon-gmail'
import IconFacebook from '~/components/icons/icon-facebook'
import IconInsta from '~/components/icons/icon-insta'

export default {
  components: { IconGmail, IconFacebook, IconInsta }
}
</script>

<style scoped lang="scss">
.footer-contacts{
  a{
    color: white;
    &:hover{
      color: $main-color;
    }
  }
}

.links{
  display: flex;
  color: white;
  li{
    color: white;
  }
}
</style>
