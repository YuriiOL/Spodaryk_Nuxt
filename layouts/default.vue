<template>
  <div>
    <nav-bar/>
    <Nuxt/>
  </div>
</template>

<script>
import NavBar from '~/components/parts/nav-bar'

export default {
  components: { NavBar },
  comments: {
    NavBar
  },
  data: () => ({
    selectedItem: 1,
    items: [
      {
        text: 'Real-Time',
        icon: 'mdi-clock'
      },
      {
        text: 'Audience',
        icon: 'mdi-account'
      },
      {
        text: 'Conversions',
        icon: 'mdi-flag'
      }
    ]
  })
}
</script>
