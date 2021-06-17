<template>
  <div class="flex try full-width">
    <div
      class="flex justify-around flex-shrink-0 w-1/2 px-16 space-x-32 flex-nowrap scroller test "
    >
      <p class="flex-shrink-0 heading heading__primary">
        MTN Ghana
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Walulel
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Sesi Technologies
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Petra Trust
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Homechow.io
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Accra Hearts of Oak
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        9+ others
      </p>
    </div>
    <div
      class="flex justify-around flex-shrink-0 w-1/2 space-x-32 scroller flex-nowrap"
    >
      <p class="flex-shrink-0 heading heading__primary">
        MTN Ghana
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Walulel
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Sesi Technologies
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Petra Trust
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Homechow.io
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        Accra Hearts of Oak
      </p>
      <p class="flex-shrink-0 heading heading__primary">
        9+ others
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
@import './assets/scss/abstracts/_mixins.scss';

.scroller {
  width: 300%;
  animation: scroll 8s linear infinite;

  @include respond(phone) {
    width: 700%;
  }
}

/* .try > * {
  flex-basis: 100%;
}
*/
/* .test > * {
  flex-basis: 200%;
} */

@keyframes scroll {
  from {
    transform: translateX(0);
  }
  to {
    transform: translateX(-150%);
  }
}
</style>
