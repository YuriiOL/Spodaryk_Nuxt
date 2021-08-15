<template>
  <div class="top-wrapper">
    <div class="top-wrapper__content">
      <h2 class="main-title animate__animated animate__fadeInUp animate__slow">
        Spodaryk
      </h2>
      <h1 class="under-title animate__animated animate__fadeIn animate__slow animate__delay-1s">
        Професійний інвентар та посуд
      </h1>
      <div class="animate__animated animate__fadeInDown">
        <div class="title-lines">
          <div class="title-lines__left" />
          <div class="title-lines__snowflake">
            ✻
          </div>
          <div class="title-lines__right" />
        </div>
        <div class="under-title-bottom">
          для кафе, барів, ресторанів та магазинів
        </div>
        <v-btn class="catalog-button">
          <a href="https://drive.google.com/drive/folders/1mE8kzWJpIlVwu0mu1M4LE89OqG5H-bcF" target="_blank">
            КАТАЛОГ
          </a>
        </v-btn>
      </div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.catalog-button {
  a{
    color: black;
  }
  &:hover {
    a{
      color: $main-color;
    }
  }
}
</style>
