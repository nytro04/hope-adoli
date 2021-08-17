<template>
  <!-- <div class="relative"> -->
  <div class="overflow-hidden">
    <LandingPage />
    <div class="md:my-72 showreal"></div>
    <Video />
    <div class="my-72"></div>
    <RecentWorks />
    <div class=" my-80"></div>

    <Jobs />

    <div class="mt-80"></div>
    <Links />
    <div class="my-40"></div>
    <!-- <Footer /> -->
    <transition name="slide">
      <div v-if="open" class="slidein">
        <UnderConstruction :close="toggle" />
      </div>
    </transition>
  </div>
</template>

<script>
export default {
  components: {
    LandingPage: () => import('~/components/LandingPage'),
    Video: () => import('~/components/Video'),
    RecentWorks: () => import('~/components/RecentWorks'),
    Links: () => import('~/components/Links'),
    Jobs: () => import('~/components/Jobs'),
    UnderConstruction: () => import('~/components/UnderConstruction')
  },

  data() {
    return {
      open: false
    }
  },
  head() {
    return {
      title: 'Hope Adoli | Portfolio Index'
    }
  },
  mounted() {
    document.body.classList.toggle('modal-open')
    this.open = true
  },

  methods: {
    toggle() {
      this.open = !this.open
      document.body.classList.toggle('modal-open')
      // refactor this
    }
  }
}
</script>

<style scoped lang="scss">
@import './assets/scss/abstracts/mixins';

@include respond(phone) {
  .showreal {
    margin: 30rem 0;
  }
}

.slidein {
  max-width: 33rem;
  /* height: 25rem; */
  /* padding: 0rem 2rem; */
  position: fixed;
  z-index: 100;
  bottom: 2rem;
  right: 1rem;
  box-shadow: 1px 1px 10px rgba(0, 0, 0, 0.5);
  transition: all 0.8s ease-in-out;

  @include respond(tab-land) {
    width: 45rem;
  }
  @include respond(tab-port) {
    width: 35rem;
  }
  @include respond(phone) {
    width: 25rem;
  }
}

.slide-enter,
.slide-leave-active {
  bottom: -100%;
}
</style>
