<template>
  <div class="landing">
    <div class="relative flex justify-between landing__main">
      <img src="~/assets/img/hope.png" alt="" class="mt-20 hero-image" />

      <span class="vertical-line"></span>

      <div class="relative mt-20 md:w-6/12">
        <!-- todo: animate border-b to load from left to right on mount -->
        <h1
          class="pb-10 md:border-b-2 md:border-white heading heading__primary sm:text-3xl"
        >
          <span class="name-line">Hope Adoli</span> <br />
          Product Designer <br />
          based in Accra, <br />
          Ghana.
        </h1>

        <div class="mt-10 content">
          <p class="">
            With 4+ years experience in building digital products that users
            love and cherish, I have worked mostly with startups in Food-tech,
            Agri-tech, Health, Fin-tech, Social Media & Education.
          </p>
          <p class="mt-5">
            I am the founder of UX Campus: A Non-Profit that seeks to inspire
            people to fall in love with UX Design, by organising free 1-2 day
            workshops across Ghana.
          </p>
        </div>
        <div class="relative svg-mobile">
          <ArrowBadgeSvg class="absolute w-20 h-20 right-2 top-2 " />
          <ArrowDownSvg class="absolute w-10 h-10 right-6 top-6" />
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
@import './assets/scss/abstracts/mixins';

.landing {
  padding: 0 2.5rem;
  /* @include respond(tab-land) {
    height: 20%;
  }
  @include respond(tab-port) {
    height: 20%;
  } */

  &__main {
    @include respond(phone) {
      display: flex;
      flex-direction: column;
      height: 70vh;
    }
  }
}

.arrow-pos {
  top: 4.7rem;

  @include respond(tab-land) {
    left: 1.7rem;
  }

  @include respond(phone) {
    bottom: 1rem;
  }
}

.content {
  @include respond(phone) {
    position: absolute;
    top: 26rem;
  }
}

.svg-mobile {
  @include respond(phone) {
    svg {
      display: none;
    }
  }
}

.hero-image {
  width: auto;
  height: 40rem;

  @include respond(tab-land) {
    height: 30rem;
    width: auto;
  }
  @include respond(tab-port) {
    height: 20rem;
    width: auto;
  }
  @include respond(phone) {
    height: auto;
    width: 15rem;
    margin: 2rem auto;

    position: absolute;
    top: 10rem;
    left: 2rem;
    z-index: -1;
  }
}

.vertical-line {
  display: inline-block;
  border-left: 2px solid white;
  // margin: 0 10px;
  height: 45rem;

  @include respond(tab-land) {
    height: 35rem;
  }
  @include respond(tab-port) {
    height: 32rem;
  }

  @include respond(phone) {
    display: none;
    /* border-bottom: 2px solid white;
    border-left: 0; */
  }
}

.name-line::after {
  background-color: #fff;
  content: '';
  display: inline-block;
  height: 0.7rem;
  right: 3rem;
  top: 6.7rem;
  position: absolute;
  vertical-align: middle;
  width: 15%;

  @include respond(tab-land) {
    right: 3.3rem;
    top: 6rem;
    width: 12%;
  }
  @include respond(tab-port) {
    right: 2.3rem;
    top: 5.7rem;
    width: 12%;
    height: 0.5rem;
  }

  @include respond(phone) {
    right: 0.8rem;
    top: 0.7rem;
    width: 30%;
    height: 0.5rem;
  }
}

p:last-child {
  @include respond(tab-port) {
    margin-bottom: 2rem;
  }
}
</style>
