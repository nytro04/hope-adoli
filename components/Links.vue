<template>
  <div class="url">
    <h2 class="text-6xl font-semibold text-right">
      Links
    </h2>
    <span class="block mt-10 mb-32 border-t-2 border-white"></span>

    <div class="">
      <h3 class="mb-10 text-7xl">
        Get In touch
      </h3>

      <button class="my-10 text-7xl">
        UX on Campus
      </button>
      <ul>
        <li
          v-for="(link, index) in links"
          :key="index"
          class="inline-block my-10 lg:text-7xl sm:text-3xl"
        >
          <nuxt-link :to="link.url">
            {{ link.name }}
            <span class="inline-block pb-8">
              <LinkSvg />
            </span>
          </nuxt-link>
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

<style></style>
