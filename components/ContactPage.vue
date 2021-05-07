<template>
  <div
    class="container h-auto mx-auto overflow-y-auto text-black bg-white contact"
  >
    <div class="h-screen px-5 py-4 md:py-10 md:px-10 lg:px-20">
      <div class="flex justify-end">
        <CloseSvg
          class="mt-5 cursor-pointer "
          style="width: 12px;"
          @click="close"
        />
      </div>

      <div class="pb-10 mt-5 border-b-2 border-black md:flex ">
        <div class="md:w-6/12 ">
          <h1 class="mb-2 text-black heading heading__primary">
            Get in <br />
            touch.
          </h1>
        </div>
        <div class="mt-6 md:mt-12 md:w-6/12">
          <p>
            Thanks in advance for reaching out! Please note that the contact
            form is for work only. If you just want to say hello, then hit me up
            on any of my social media handles.
          </p>
        </div>
      </div>

      <ul class="flex justify-between py-4 border-b-2 border-black md:py-8">
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
              <LinkSvg />
            </span>
          </a>
        </li>
      </ul>

      <form class="mt-8 lg:mt-20 md:mt-10" @submit.prevent="handleContact">
        <div class="md:flex">
          <div class="md:w-1/2">
            <input
              id="firstName"
              name="firstName"
              class="inline-block w-full px-3 py-1 mb-3 bg-gray-200 md:py-3"
              type="text"
              placeholder="First name"
            />

            <input
              id="email"
              name="email"
              class="inline-block w-full px-3 py-1 mb-3 bg-gray-200 md:py-3 "
              type="email"
              placeholder="Email Address"
              required
            />

            <div>
              <select
                id="interest"
                name="interest"
                class="inline-block w-full px-2 py-2 mb-3 bg-gray-200 md:py-3 "
              >
                <option value="">
                  Interested in...
                </option>
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
                  General Inquiry
                </option>
              </select>
            </div>
            <div>
              <select
                id="interest"
                name="interest"
                class="inline-block w-full px-2 py-2 mb-3 bg-gray-200 md:py-3"
              >
                <option value="">
                  What's your budget range?
                </option>
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
          <div class="md:w-1/2 md:ml-8">
            <textarea
              id=""
              name=""
              cols="30"
              rows="3"
              required
              placeholder="Tell me more about your project"
              class="w-full px-3 py-2 mb-3 text-sm bg-gray-200 resize-none"
            ></textarea>
            <div class="mt-2 md:text-right">
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
@import './assets/scss/abstracts/mixins';

.contact {
  @include respond(phone) {
    padding: 0 3rem;
  }

  p {
    font-size: 0.8rem;
  }
}

.link-text {
  font-size: 2.5rem;

  @include respond(tab-land) {
    font-size: 1.5rem;
  }

  @include respond(tab-port) {
    font-size: 1.5rem;
  }

  @include respond(phone) {
    font-size: 1rem;
  }
}

.arrow-icon {
  position: absolute;
  top: 13px;
  right: -1.1rem;

  svg {
    width: 12px;
    @include respond(tab-land) {
      width: 10px;
    }

    @include respond(tab-port) {
      width: 8px;
    }

    @include respond(phone) {
      width: 6px;
    }
  }

  @include respond(tab-land) {
    top: 5px;
    right: -0.8rem;
  }

  @include respond(tab-port) {
    top: 8px;
    right: -0.9rem;
  }

  @include respond(phone) {
    top: 1px;
    right: -0.5rem;
  }
}
</style>
