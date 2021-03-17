<template>
  <nav class="flex justify-between py-4 border-b-2 border-white">
    <h3 class="heading heading__tertiary">
      HOPE ADOLI
      <span v-if="$nuxt.$route.path !== '/'" class="text-gray-400"
        >/ {{ page }}</span
      >
    </h3>
    <h3 class="heading heading__tertiary">
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
    }
  }
}
</script>

<style></style>
