<template>
  <div>
    <main-small-banner
      :title="'Контакти'"
    />
    <info-block />
  </div>
</template>

<script>
import MainSmallBanner from '~/components/banners/main-small-banner'
import InfoBlock from '~/components/contacts/info-block'
export default {
  components: { InfoBlock, MainSmallBanner }
}
</script>

<style scoped>

</style>
