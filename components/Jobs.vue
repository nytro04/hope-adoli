<template>
  <div class="full-width ">
    <div class="flex px-16 space-x-32 scroller whitespace-nowrap">
      <p class="heading heading__primary">
        MTN Ghana
      </p>
      <p class="heading heading__primary">
        Walulel
      </p>
      <p class="heading heading__primary">
        Sesi Technologies
      </p>
      <p class="heading heading__primary">
        Homechow.io
      </p>
      <p class="heading heading__primary">
        Accra Hearts of Oak
      </p>
      <p class="heading heading__primary">
        9+ others
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped>
.scroller {
  animation: scroll 15s infinite;
}

@keyframes scroll {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-180%);
  }
}
</style>
