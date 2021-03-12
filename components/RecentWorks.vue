<template>
  <div class="recent-works">
    <h2 class="text-6xl font-semibold text-right">
      Recent works
    </h2>
    <span class="block mt-10 mb-32 border-t-2 border-white"></span>

    <div class="card-container">
      <div class="card-member member-1">
        <div class="bg-red-200 jarallax">
          <img src="~/assets/img/GrainMate.png" alt="" class="jarallax-img" />
          <div class="para-img"></div>
        </div>
        <h3 class="mt-10 mb-3 text-3xl font-semibold">
          GrainMate mobile
        </h3>
        <p>
          GrainMate app is supercharging African farmers and agribusinesses with
          the tools and resources they need to get to the next level ⚡️
        </p>
      </div>
      <div class="card-member member-2">
        <div class="bg-red-200 jarallax">
          <img
            src="~/assets/img/Wacomm-mobile.png"
            alt=""
            class="jarallax-img wa-bg"
          />
          <div class="para-img"></div>
        </div>
        <h3 class="mt-10 mb-3 text-3xl font-semibold">
          Wacomm mobile
        </h3>
        <p>
          The Geo-social property management app that connects property owners
          and their tenants.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  components: {}
}
</script>

<style scoped lang="scss">
.card-container {
  height: 80vh;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  column-gap: 15rem;
  /* grid-template-rows: auto 1fr 1fr 2fr 1fr 1fr; */
  grid-template-rows: repeat(6, 1fr);

  .para-img {
    height: 30rem;
  }
}

.wa-bg {
  background-color: #192a49;
}

.member-1 {
  grid-row-start: 1;
  grid-column-start: 1;
  grid-row-end: 5;
}
.member-2 {
  grid-row-start: 2;
  grid-column-start: 2;
  grid-row-end: 5;
}

.recent-bg {
  background-color: red;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
