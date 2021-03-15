<template>
  <div class="">
    <nav class="flex justify-between py-4 border-b-2 border-white">
      <h3 class="heading heading__tertiary">
        HOPE ADOLI
      </h3>
      <h3 class="heading heading__tertiary">
        contact me
      </h3>
    </nav>

    <div class="relative flex justify-between">
      <img src="~/assets/img/hope.png" alt="" class="w-5/12 mt-20 hero-image" />

      <span class="vertical-line"></span>

      <div class="w-6/12 mt-20">
        <h1 class="border-b-2 border-white heading heading__primary">
          <span class="name-line">Hope Adoli</span> <br />
          Product Designer <br />
          based in Accra, <br />
          Ghana.
        </h1>

        <div class="flex justify-between mt-10">
          <div class="w-8/12">
            <p>
              With over 3 years experience in building digital products that
              users love and cherish, I have worked mostly with startups in Food
              tech, Agri-tech, Health, Fin-tech, Social Media & Education.
            </p>
            <p class="mt-8">
              I am the founder of UX Campus: An Non Profit that seeks to inspire
              people to fall in love with UX Design, by organising free 1-2 day
              workshops across Ghana.
            </p>
          </div>
          <div class="relative ml-20">
            <ArrowBadgeSvg class="w-8/12" />
            <ArrowDownSvg class="absolute h-12 arrow-pos left-10 " />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import ArrowBadgeSvg from '~/assets/svgs/scroll-down-badge.svg?inline'
import ArrowDownSvg from '~/assets/svgs/scroll-down-arrow.svg?inline'

export default {
  components: {
    ArrowDownSvg,
    ArrowBadgeSvg
  }
}
</script>

<style scoped lang="scss">
.arrow-pos {
  top: 4.7rem;
}

.hero-image {
  width: auto;
  height: 40rem;
}

.vertical-line {
  display: inline-block;
  border-left: 2px solid white;
  // margin: 0 10px;
  height: 45rem;
}

.name-line::after {
  background-color: #fff;
  content: '';
  display: inline-block;
  height: 0.7rem;
  right: 3.5rem;
  top: 7.4rem;
  position: absolute;
  vertical-align: middle;
  width: 15%;
}
</style>
