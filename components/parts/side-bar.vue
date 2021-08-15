<template>
  <v-navigation-drawer
    v-model="drawer"
    class="side-bar"
    fixed
    dark
  >
    <v-list
      nav
      dense
    >
      <v-list-item-group
        active-class="deep-purple--text text--accent-4"
      >
        <v-list-item link to="/">
          <v-list-item-title>Головна</v-list-item-title>
        </v-list-item>

        <v-list-item link to="/contacts">
          <v-list-item-title>Контакти</v-list-item-title>
        </v-list-item>

        <v-list-item link to="/about">
          <v-list-item-title>
            Про нас
          </v-list-item-title>
        </v-list-item>
      </v-list-item-group>
    </v-list>
  </v-navigation-drawer>
</template>

<script>
export default {
  data: () => ({
    drawer: false
  }),
  methods: {
    toggle () {
      this.drawer = true
    }
  }
}
</script>

<style scoped>
.side-bar{
  background-color: black;
}
</style>
