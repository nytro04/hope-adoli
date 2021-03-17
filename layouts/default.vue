<template>
  <div class="container mx-auto">
    <Navbar />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  components: {
    Navbar: () => import('~/components/Navbar'),
    Footer: () => import('~/components/Footer')
  }
}
</script>

<style></style>
