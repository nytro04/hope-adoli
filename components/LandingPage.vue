<template>
  <div class="">
    <nav class="flex justify-between py-4 border-b-2 border-white">
      <h3 class="heading heading__tertiary">
        HOPE ADOLI
      </h3>
      <h3 class="heading heading__tertiary">
        contact info
      </h3>
    </nav>

    <div class="relative flex justify-between">
      <img src="~/assets/img/hope.png" alt="" class="mt-20 hero-image" />

      <span class="vertical-line"></span>

      <div>
        <h1 class="mt-20 heading heading__primary">
          <span class="name-line">Hope Adoli</span> <br />
          Product Designer <br />
          based in Accra, <br />
          Ghana.
        </h1>

        <div class="flex">
          <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Natus,
            fuga.
          </p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// import ArrowDownSvg from '~/assets/svgs/play-showreel-badge.svg?inline'

export default {
  components: {
    // ArrowDownSvg
  }
}
</script>

<style scoped lang="scss">
.hero-image {
  width: 30rem;
  height: 40rem;
}

.vertical-line {
  display: inline-block;
  border-left: 2px solid white;
  margin: 0 10px;
  height: 45rem;
}

.name-line::after {
  background-color: #fff;
  content: '';
  display: inline-block;
  height: 0.7rem;
  right: 0.1rem;
  top: 7.4rem;
  position: absolute;
  vertical-align: middle;
  width: 15%;
}
</style>
