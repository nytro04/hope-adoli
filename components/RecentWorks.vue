<template>
  <div class="recent-works">
    <h2 class="mr-5 font-semibold text-right heading heading__primary">
      Recent works
    </h2>
    <span class="block mt-10 mb-32 border-t-2 border-white"></span>

    <div class="md:mb-20 md:flex md:items-center md:justify-between">
      <nuxt-link to="grainmate" class="md:w-5/12 ">
        <img src="~/assets/img/new/GrainMate.png" alt="" class="" />

        <div class="pb-20 slider">
          <h3
            class="mt-10 mb-3 font-semibold md:text-2xl lg:text-3xl text-c-mob move"
          >
            GrainMate mobile
          </h3>
          <p class="">
            GrainMate app is supercharging African farmers and agribusinesses
            with the tools and resources they need to get to the next level ⚡️
          </p>
        </div>
      </nuxt-link>
      <nuxt-link to class="md:w-5/12 md:mt-20">
        <img src="~/assets/img/new/Wacomm.png" alt="" class="" />

        <div class="pb-20 slider">
          <h3
            class="mt-10 mb-3 font-semibold md:text-2xl lg:text-3xl text-c-mob "
          >
            Wacomm mobile
          </h3>

          <p :class="{ active: hover }" class="move">
            The Geo-social property management app that connects property owners
            and their tenants.
          </p>
        </div>
      </nuxt-link>
    </div>

    <div class="md:mb-20 md:flex md:items-center md:justify-between">
      <nuxt-link to class="md:w-5/12">
        <img src="~/assets/img/new/Adiutor.png" alt="" class="" />

        <div class="pb-20 slider">
          <h3
            class="mt-10 mb-3 font-semibold md:text-2xl lg:text-3xl text-c-mob "
          >
            Adiutor
          </h3>
          <p class="">
            Aduitor is attempting to redefine how educational institutions are
            managed in Ghana and Africa as a whole.
          </p>
        </div>
      </nuxt-link>
      <nuxt-link to class="md:w-5/12 md:mt-20">
        <img src="~/assets/img/new/Homechow.png" alt="" class="" />

        <div class="pb-20 slider">
          <h3
            class="mt-10 mb-3 font-semibold md:text-2xl lg:text-3xl text-c-mob "
          >
            Homechow
          </h3>
          <p class="">
            One of Ghana’s best & most promising food delivery startups in 2019
          </p>
        </div>
      </nuxt-link>
    </div>

    <div class="md:mb-20 md:flex md:items-center md:justify-between">
      <nuxt-link to="#" class="md:w-5/12">
        <img src="~/assets/img/new/Farm-for-me.png" alt="" class="" />

        <div class="pb-20 slider">
          <h3
            class="mt-10 mb-3 font-semibold md:text-2xl lg:text-3xl text-c-mob "
          >
            A Farm For Me web
          </h3>

          <p class="">
            A Farm For Me is a web app for Africans to invest in virtual farms
            and and earn profits.
          </p>
        </div>
      </nuxt-link>
      <nuxt-link to="#" class="md:w-5/12 md:mt-20">
        <img src="~/assets/img/new/Microbis.png" alt="" class="" />

        <div class="pb-20 slider">
          <h3
            class="mt-10 mb-3 font-semibold md:text-2xl lg:text-3xl text-c-mob "
          >
            MicroBis web
          </h3>

          <!-- <p> -->
          <p class="">
            MicroBis helps laboratory scientist to detect bacteria in samples
            and suggests possible antibiotics it will be susceptible to.
          </p>
        </div>
      </nuxt-link>
    </div>
  </div>
</template>

<script>
export default {
  components: {},

  data() {
    return {
      hover: false
    }
  }
}
</script>

<style scoped lang="scss">
@import './assets/scss/abstracts/_mixins.scss';

.text-c-mob {
  @include respond(phone) {
    /* text-align: center; */
    margin-left: 2rem;
  }
}

.card-container {
  height: 80vh;
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  column-gap: 15rem;
  /* grid-template-rows: auto 1fr 1fr 2fr 1fr 1fr; */
  grid-template-rows: repeat(6, 1fr);

  @include respond(tab-land) {
    column-gap: 8rem;
    height: 90vh;
    margin-bottom: 0;
  }

  @include respond(tab-port) {
    column-gap: 8rem;
    height: 70vh;
    margin-bottom: 0;
  }

  @include respond(phone) {
    display: block;
    /* height: 150vh; */
    height: auto;
  }

  .para-img {
    height: 35rem;

    @include respond(tab-land) {
      height: 28rem;
    }

    @include respond(tab-port) {
      height: 28rem;
    }

    @media (width: 812px) {
      height: 8rem;
    }

    @include respond(phone) {
      height: 25rem;
      width: 80%;
    }
  }

  /* @include respond(tab-port) {
    height: 4.875rem;
  } */
  /* @include respond(phone) {
    height: 4.875rem;
  } */

  /* position: relative; */
}

/* .line-enter-active,
.line-leave-enter {
  width: 100%;

  transition: all 0.3s linear;
}

.line-enter,
.line-leave-to {
  transition: all 0.3s linear;

  width: 0;
}

.try {
  border: 2px solid #fff;
  overflow: hidden;
  margin-top: 5rem;
} */

.adiutor {
  background-color: #8c83b0;
}
.grain {
  background-color: #f6dacc;
}
.farm {
  background-color: #84ae73;
}

.wacomm {
  background-color: #192a49;
}

.homechow {
  background-color: #e1c098;
}

.microbis {
  background-color: #c7e4e5;
}

.member-1 {
  grid-row-start: 1;
  grid-column-start: 1;
  grid-row-end: 5;

  @include respond(phone) {
  }
}
.member-2 {
  grid-row-start: 2;
  grid-column-start: 2;
  grid-row-end: 5;

  @include respond(phone) {
  }
}

.recent-bg {
  background-color: red;
  background-size: cover;
  background-repeat: no-repeat;
}
</style>
