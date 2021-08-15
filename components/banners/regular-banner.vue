<template>
  <div class="pause-place pause-place-top" :style="{backgroundImage: image}">
    <div class="smallTitleAnimation">
      <div class="main-title">
        The latest
      </div>
      <div class="under-title color-white">
        DESIGN
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    image: {
      type: String,
      default: ''
    }
  },
  computed: {

  }
}
</script>

<style scoped lang="scss">
.under-title{
  color: white;
}
</style>
