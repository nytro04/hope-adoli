<template>
  <div class="container mx-auto text-black bg-white contact">
    <div class="h-screen p-5 px-20 py-10">
      <div class="flex justify-end">
        <CloseSvg
          class="mt-5 cursor-pointer "
          style="width: 12px;"
          @click="close"
        />
      </div>

      <div class="flex pb-10 mt-5 border-b-2 border-black">
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
        <li v-for="(link, index) in links" :key="index" class="relative">
          <a
            class="font-bold link-text"
            :href="link.url"
            target="_blank"
            rel="noopener noreferrer"
          >
            <span class="">
              {{ link.name }}
            </span>
            <span class="arrow-icon">
              <LinkSvg style="width: 12px;" />
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
                  UI/UX Design
                </option>
                <option value="">
                  UX Audit
                </option>
                <option value="">
                  UX Consultation
                </option>
                <option value="">
                  General Enquiry
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
                  Less than $3,500
                </option>
                <option value="">
                  $3,600 - $5,000
                </option>
                <option value="">
                  $6,000 - $9,000
                </option>
                <option value="">
                  More than $10,000
                </option>
                <option value="">
                  No budget yet 🙁
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
import CloseSvg from '~/assets/svgs/x.svg?inline'

export default {
  components: {
    LinkSvg,
    CloseSvg
  },
  props: {
    close: {
      type: Function,
      default: () => ({})
    }
  },
  data() {
    return {
      open: false,
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
    // close() {
    //   this.$emit('close-slide')
    // },

    handleContact() {}
  }
}
</script>

<style scoped lang="scss">
.link-text {
  font-size: 2.5rem;
}

.arrow-icon {
  position: absolute;
  top: 13px;
  right: -1.1rem;
}
</style>
