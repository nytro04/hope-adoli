<template>
  <div class="container mx-auto">
    <Navbar :page="currentRoute" />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  components: {
    Navbar: () => import('~/components/Navbar'),
    Footer: () => import('~/components/Footer')
  },

  computed: {
    currentRoute() {
      const name = this.$nuxt.$route.path
        .split('/')
        .join('')
        .split('-')
        .join('')
        .toUpperCase()

      return name
    }
  }
}
</script>

<style></style>
