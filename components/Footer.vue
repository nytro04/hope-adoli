<template>
  <div class="footer">
    <div class="justify-between py-5 border-t-2 border-white md:flex res-mob">
      <p class="">
        &copy; uxkafui
      </p>
      <p class="text-gray-500">
        2021 folio
      </p>
      <!-- <div class=""> -->
      <ul class="justify-between md:flex ">
        <li v-for="(link, index) in links" :key="index">
          <a
            class="ml-10"
            :href="link.url"
            target="_blank"
            rel="noopener noreferrer"
          >
            {{ link.name }}
          </a>
        </li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      links: [
        // {
        //   name: 'contact',
        //   url: '/get-in-touch'
        // },
        {
          name: 'Twitter',
          url: 'https://twitter.com/uxkafui'
        },

        {
          name: 'Instagram',
          url: 'https://instagram.com/uxkafui'
        },
        {
          name: 'LinkedIn',
          url: 'https://linkedin.com/in/hopeadoli'
        }
      ]
    }
  }
}
</script>

<style scoped lang="scss">
@import './assets/scss/abstracts/mixins';

p {
  @include respond(phone) {
    font-size: 0.42rem;
  }
}

.res-mob > * {
  @include respond(phone) {
    margin: 0 1rem;
  }
}

.footer {
  @include respond(phone) {
    font-size: 0.42rem;
  }
}
</style>
