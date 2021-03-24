<template>
  <div class="container mx-auto text-black bg-white contact">
    <div class="px-20 pt-20 pb-10 sidenav">
      <i
        class="mt-10 cursor-pointer hover:bg-black hover:text-white closebtn"
        @click="close()"
      >
        &times;
      </i>

      <div class="flex pb-10 mt-20 border-b-2 border-black">
        <div class="w-6/12">
          <h1 class="text-black heading heading__primary">
            Get in <br />
            touch.
          </h1>
        </div>
        <div class="w-6/12">
          <p>
            Thanks in advance for reaching out! Please note that the contact
            form is for work only. If you just want to say hello, then hit me up
            on any of my social media handles.
          </p>
        </div>
      </div>

      <ul class="flex justify-between py-12 border-b-2 border-black">
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

      <form class="mt-10" @submit.prevent="">
        <div class="flex">
          <div class="">
            <input
              id="firstName"
              name="firstName"
              class="inline-block mb-3"
              type="text"
              placeholder="First name"
              required
            />

            <input
              id="lastName"
              name="lastName"
              class="inline-block mb-3"
              type="text"
              placeholder="Last name"
              required
            />

            <select id="interest" name="interest" class="inline-block">
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
            <select id="interest" name="interest" class="inline-block">
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
          <div class="">
            <textarea
              id=""
              name=""
              cols="30"
              rows="7"
              class="resize-none"
            ></textarea>
          </div>
        </div>

        <div class="text-right">
          <button class=" btn btn__black">
            Send message
          </button>
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
          url: '/get-in-touch'
        },

        {
          name: 'Instagram',
          url: '/get-in-touch'
        },
        {
          name: 'Linkedin',
          url: '/get-in-touch'
        }
      ]
    }
  },
  methods: {
    close() {
      this.$emit('close-slide')
    }
  }
}
</script>

<style scoped lang="scss">
.link-text {
  font-size: 2.5rem;
}
</style>
