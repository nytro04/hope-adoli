<template>
  <div class="my-40 grain-mate">
    <div class="flex justify-between">
      <div class="w-6/12">
        <h1 class="heading heading__primary">
          GrainMate <br />
          mobile app
        </h1>
        <p class="mt-8 text-gray-400">
          Sesi technologies • 2020
        </p>
      </div>

      <div class="w-6/12">
        <h3 class="mb-6 text-4xl font-bold text-gray-400">
          Overview
        </h3>
        <p class="text-gray-400">
          Meet GrainMate app: A companion of GrainMate moisture meter. While the
          moisture meter is used to measure the moisture content in grains, the
          app uses the result to suggest a solution. But that’s not all. The
          app’s Learn feature curates mini lessons on Post Harvest Loss (PHL)
          and how to prevent/manage it. It also has a marketplace for
          agribusinesses to sell agricultural products.
        </p>

        <div class="mt-8">
          <nuxt-link to="">
            Download on Google Playstore
          </nuxt-link>
        </div>
      </div>
    </div>

    <div class="full-width">
      <div class="mt-20 grain-bg"></div>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style lang="scss" scoped>
.grain-bg {
  background-image: url('~/assets/img/hero-section-img.png');
  height: 90vh;
  width: 100%;
  background-size: cover;
  background-position: center;
  background-color: #11905c;
}

.full-width {
  margin-left: -5rem;
  margin-right: -5rem;
}
</style>
