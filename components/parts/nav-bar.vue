<template>
  <div>
    <v-app-bar
      class="nav"
      dark
      fixed
      color="black"
    >
      <v-app-bar-nav-icon class="nav-icon" @click="toggle" />

      <div class="main-logo">
        <NuxtLink to="/">
          <img src="/images/Spodaryk_Logo.png" alt="Logo">
        </NuxtLink>
      </div>

      <v-tabs
        class="nav-list"
        dark
        :centered="true"
      >
        <v-tab link to="/">
          Головна
        </v-tab>

        <v-tab link to="/contacts">
          Контакти
        </v-tab>

        <v-tab link to="/about">
          Про нас
        </v-tab>
      </v-tabs>

      <div>
        <v-btn icon small href="https://www.instagram.com/spodaryk.group/" target="_blank">
          <icon-insta />
        </v-btn>

        <v-btn icon small href="https://www.facebook.com/spodaryk.group" target="_blank">
          <icon-facebook />
        </v-btn>
        <v-btn icon small link href="mailto:spodarykgroup@gmail.com" target="_blank">
          <icon-gmail />
        </v-btn>
      </div>
    </v-app-bar>

    <side-bar ref="sideBar" />
  </div>
</template>

<script>
import SideBar from '~/components/parts/side-bar'
import IconInsta from '~/components/icons/icon-insta'
import IconFacebook from '~/components/icons/icon-facebook'
import IconGmail from '~/components/icons/icon-gmail'
export default {
  components: { IconGmail, IconFacebook, IconInsta, SideBar },
  methods: {
    toggle () {
      this.$refs.sideBar.toggle()
    }
  }
}
</script>

<style scoped>
.nav {
  padding: 0 50px;
}
.theme--dark.v-app-bar.v-toolbar.v-sheet {
  background-color: black;
}
.nav >>> .v-toolbar__content, .v-toolbar__extension{
  justify-content: space-between;
}

.nav-list {
  width: auto;
}

.nav-icon {
  display: none;
}

.nav-list >>> .v-slide-group__content {
  justify-content: center;
}

.main-logo {
  height: 100%;
}

@media only screen and (max-width: 992px) {
  .nav-list {
    display: none;
  }

  .nav-icon {
    display: block;
  }
}

@media only screen and (max-width: 576px) {
  .nav {
    padding: 0 10px;
  }
}
</style>
