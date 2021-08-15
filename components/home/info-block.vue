<template>
  <div :class="['about-line-container', revers ? 'catalog-line-container' : '']">
    <div class="about-line-container__left">
      <h2 class="about-title">
        <slot name="mainTitle" />
      </h2>
      <p class="about-small-title">
        <slot name="smallTitle" />
      </p>
      <p class="about-text">
        <slot name="text" />
      </p>
      <v-btn class="link-button" :href="link.url">
        {{ link.name }}
      </v-btn>
    </div>
    <div class="about-line-container__right">
      <img :src="images" alt="dishes">
    </div>
  </div>
</template>

<script>
export default {
  props: {
    link: {
      type: Object,
      default: () => ({})
    },
    revers: {
      type: Boolean,
      default: false
    },
    images: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped lang="scss">
.link{
  color: $main-color;
}

.link-button{
  margin-top: 10px;
}
</style>
