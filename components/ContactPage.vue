<template>
  <div class="container mx-auto text-black bg-white contact">
    <div class="px-20 pt-10 pb-10 sidenav">
      <div class="text-right">
        <i
          class="mt-10 text-4xl cursor-pointer hover:bg-black hover:text-white"
          @click="close()"
        >
          &times;
        </i>
      </div>

      <div class="flex pb-10 mt-10 border-b-2 border-black">
        <div class="w-6/12 ">
          <h1 class="mb-2 text-black heading heading__primary">
            Get in <br />
            touch.
          </h1>
        </div>
        <div class="w-6/12 mt-12 text-sm">
          <p>
            Thanks in advance for reaching out! Please note that the contact
            form is for work only. If you just want to say hello, then hit me up
            on any of my social media handles.
          </p>
        </div>
      </div>

      <ul class="flex justify-between py-8 border-b-2 border-black">
        <li v-for="(link, index) in links" :key="index" class="">
          <a
            class="font-bold link-text"
            :href="link.url"
            target="_blank"
            rel="noopener noreferrer"
          >
            {{ link.name }}
            <span class="inline-block pb-5">
              <LinkSvg />
            </span>
          </a>
        </li>
      </ul>

      <form class="mt-20" @submit.prevent="handleContact">
        <div class="flex">
          <div class="w-1/2">
            <input
              id="firstName"
              name="firstName"
              class="inline-block w-full px-3 py-2 mb-3 bg-gray-200"
              type="text"
              placeholder="First name"
              required
            />

            <input
              id="email"
              name="email"
              class="inline-block w-full px-3 py-2 mb-3 bg-gray-200 "
              type="email"
              placeholder="Email Address"
              required
            />

            <div>
              <select
                id="interest"
                name="interest"
                class="inline-block w-full px-3 py-3 mb-3 bg-gray-200 "
              >
                <option value="">
                  Interested In ?
                </option>
                <option value="">
                  Interested In
                </option>
                <option value="">
                  Interested In ?
                </option>
                <option value="">
                  Interested In ?
                </option>
              </select>
            </div>
            <div>
              <select
                id="interest"
                name="interest"
                class="inline-block w-full px-3 py-3 mb-3 bg-gray-200"
              >
                <option value="">
                  What's your budget range
                </option>
                <option value="">
                  Interested In
                </option>
                <option value="">
                  Interested In ?
                </option>
                <option value="">
                  Interested In ?
                </option>
              </select>
            </div>
          </div>
          <div class="w-1/2 ml-8">
            <textarea
              id=""
              name=""
              cols="30"
              rows="5"
              placeholder="Tell me more about your project"
              class="w-full px-3 py-2 mb-3 text-sm bg-gray-200 resize-none"
            ></textarea>
            <div class="mt-2 text-right">
              <button class=" btn btn__black">
                Send message
              </button>
            </div>
          </div>
        </div>
      </form>
    </div>
  </div>
</template>

<script>
import LinkSvg from '~/assets/svgs/arrow-up-right-2.svg?inline'

export default {
  components: {
    LinkSvg
  },
  data() {
    return {
      links: [
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
  },
  methods: {
    close() {
      this.$emit('close-slide')
    },

    handleContact() {}
  }
}
</script>

<style scoped lang="scss">
.link-text {
  font-size: 2.5rem;
}
</style>
