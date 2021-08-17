<template>
  <div class="top-wrapper top-wrapper-contact">
    <div class="top-wrapper__content">
      <h1 class="main-title animate__animated">
        Spodaryk
      </h1>
      <h2 class="under-title animate__animated">
        {{ title }}
      </h2>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    title: {
      type: String,
      default: ''
    }
  }
}
</script>

<style scoped>
.top-wrapper-contact{
  margin-top: 50px;
  min-height: 50vh;
}
</style>
