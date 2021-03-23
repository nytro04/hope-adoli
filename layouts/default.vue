<template>
  <div class="container mx-auto">
    <transition name="slide">
      <ContactPage v-show="showSlideMenu" @close-slide="closeSlideMenu" />
    </transition>
    <Navbar :page="currentRoute" @open-slide="openSlideMenu()" />
    <nuxt />
    <Footer />
  </div>
</template>

<script>
export default {
  components: {
    Navbar: () => import('~/components/Navbar'),
    Footer: () => import('~/components/Footer'),
    ContactPage: () => import('~/components/ContactPage')
  },

  data() {
    return {
      showSlideMenu: false
    }
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
  },

  methods: {
    openSlideMenu() {
      this.showSlideMenu = true
    },

    closeSlideMenu() {
      this.showSlideMenu = false
    }
  }
}
</script>

<style></style>
