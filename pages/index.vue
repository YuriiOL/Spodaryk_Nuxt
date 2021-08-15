<template>
  <div>
    <main-banner />
    <info-block />
    <regular-banner />
  </div>
</template>
<script>
import MainBanner from '~/components/banners/main-banner'
import InfoBlock from '~/components/home/info-block'
import RegularBanner from '~/components/banners/regular-banner'
export default {
  components: { RegularBanner, InfoBlock, MainBanner }
}
</script>
