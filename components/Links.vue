<template>
  <div class="url">
    <h2 class="font-semibold text-right heading heading__primary">
      Links
    </h2>
    <span class="block mt-10 mb-32 border-t-2 border-white"></span>

    <div class="">
      <h3 class="mb-10 cursor-pointer sm:ml-5 heading__links" @click="toggle">
        Get In touch
      </h3>

      <button class="my-10 sm:ml-5 heading__links">
        UX on Campus
      </button>

      <ul>
        <li
          v-for="(link, index) in links"
          :key="index"
          class="inline-block my-10 heading__links"
        >
          <a
            class=""
            :href="link.url"
            target="_blank"
            rel="noopener noreferrer"
          >
            {{ link.name }}
            <span class="inline-block pb-8 svg-icons">
              <LinkSvg />
            </span>
          </a>
        </li>
      </ul>
    </div>

    <transition name="slide">
      <div v-if="open" class="slidein">
        <ContactPage :close="toggle" />
      </div>
    </transition>
  </div>
</template>

<script>
import LinkSvg from '~/assets/svgs/arrow-up-right.svg?inline'

export default {
  components: {
    LinkSvg,
    ContactPage: () => import('~/components/ContactPage')
  },
  data() {
    return {
      open: false,
      links: [
        {
          name: 'Donwload free design resources',
          url: '/get-in-touch'
        },
        {
          name: 'Learn UX Design (paid)',
          url: '/get-in-touch'
        }
      ]
    }
  },

  methods: {
    toggle() {
      this.open = !this.open
      // refactor this
      document.body.classList.toggle('modal-open')
    }
  }
}
</script>

<style lang="scss" scoped>
@import './assets/scss/abstracts/mixins';

.svg-icons {
  @include respond(phone) {
    height: 0.7rem;
  }
}

.slidein {
  max-width: 60rem;

  position: fixed;
  z-index: 100;
  top: 0;
  right: 0;
  box-shadow: 1px 1px 10px rgba(0, 0, 0, 0.5);
  transition: all 0.5s ease-in-out;

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
  right: -100%;
}
</style>
