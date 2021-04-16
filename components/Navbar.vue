<template>
  <nav class="flex justify-between py-4 border-b-2 border-white nav--main">
    <nuxt-link to="/" class="heading heading__tertiary">
      HOPE ADOLI
      <span v-if="$nuxt.$route.path !== '/'" class="text-gray-400">
        / {{ page }}
      </span>
    </nuxt-link>
    <h3 class="cursor-pointer heading heading__tertiary" @click="open">
      contact me
    </h3>

    <!-- {{ $nuxt.$route.path }} -->
  </nav>
</template>

<script>
export default {
  props: {
    page: {
      type: String,
      default: ''
    },
    open: {
      type: Function,
      default: () => ({})
    }
  },

  methods: {}
}
</script>

<style scoped lang="scss">
@import './assets/scss/abstracts/_mixins.scss';

.nav--main {
  @include respond(phone) {
    margin: 2rem 1rem 0 1rem;
  }
}
</style>
