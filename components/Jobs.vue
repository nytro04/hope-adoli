<template>
  <div class="full-width ">
    <div
      class="flex px-16 space-x-32 scroller heading heading__primary whitespace-nowrap"
    >
      <p>MTN Ghana</p>
      <p>Walulel</p>
      <p>Sesi Technologies</p>
      <p>Homechow.io</p>
      <p>Accra Hearts of Oak</p>
      <p>9+ others</p>
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
