<template>
  <div class="container mx-auto">
    <transition name="slide">
      <div v-if="open" class="slidein">
        <ContactPage :close="toggle" />
      </div>
    </transition>
    <Navbar :page="currentRoute" :open="toggle" />
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
      open: false
    }
  },

  computed: {
    currentRoute() {
      const name = this.$nuxt.$route.path
        .split('/')
        .join('')
        // .split('-')
        // .join('')
        .toUpperCase()

      return name
    }
  },

  methods: {
    toggle() {
      this.open = !this.open
    }
  }
}
</script>

<style scoped>
.slidein {
  max-width: 50rem;

  position: fixed;
  z-index: 100;
  top: 0;
  right: 0;
  box-shadow: 1px 1px 10px rgba(0, 0, 0, 0.5);
  transition: all 0.5s ease-in-out;
}

.slide-enter,
.slide-leave-active {
  right: -100%;
}
</style>
