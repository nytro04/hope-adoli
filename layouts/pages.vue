<template>
  <div class="">
    <transition name="slide">
      <div v-if="open" class="slidein">
        <ContactPage :close="toggle" />
      </div>
    </transition>
    <div class="container mx-auto sm:px-10">
      <Navbar :page="currentRoute" :open="toggle" />
    </div>
    <nuxt />
    <div class="container mx-auto sm:px-10">
      <Footer />
    </div>
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

<style scoped lang="scss">
@import '../assets/scss/abstracts/_mixins.scss';

.slidein {
  max-width: 60rem;

  position: fixed;
  z-index: 100;
  top: 0;
  right: 0;
  box-shadow: 1px 1px 10px rgba(0, 0, 0, 0.5);
  transition: all 0.5s ease-in-out;

  @include respond(tab-land) {
    width: 45rem;
  }
  @include respond(tab-port) {
    width: 35rem;
  }
  @include respond(phone) {
    width: 25rem;
  }
}

.slide-enter,
.slide-leave-active {
  right: -100%;
}
</style>
