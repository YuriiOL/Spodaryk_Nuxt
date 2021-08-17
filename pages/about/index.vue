<template>
  <div>
    <main-small-banner
      :title="'Про компанію'"
    />
    <info-block />
  </div>
</template>

<script>
import MainSmallBanner from '~/components/banners/main-small-banner'
import InfoBlock from '~/components/about/info-block'

export default {
  components: { InfoBlock, MainSmallBanner }
}
</script>

<style scoped>

</style>
