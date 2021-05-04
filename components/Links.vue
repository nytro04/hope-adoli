<template>
  <div class="url">
    <h2 class="font-semibold text-right heading heading__primary">
      Links
    </h2>
    <span class="block mt-10 mb-32 border-t-2 border-white"></span>

    <div class="">
      <h3 class="mb-10 sm:ml-5 heading__links">
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
  </div>
</template>

<script>
import LinkSvg from '~/assets/svgs/arrow-up-right.svg?inline'

export default {
  components: {
    LinkSvg
  },
  data() {
    return {
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
</style>
