<template>
  <div>
    <nav-bar />
    <Nuxt />
    <Footer />
  </div>
</template>

<script>
import NavBar from '~/components/parts/nav-bar'
import Footer from '~/components/parts/footer'

export default {
  comments: {
    NavBar,
    Footer
  },
  components: { NavBar, Footer },
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
