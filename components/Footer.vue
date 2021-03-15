<template>
  <div class="footer">
    <div class="flex justify-between py-5 border-t-2 border-white">
      <p class="w-1/4">
        &#169; uxkafui
      </p>
      <p>2021 folio</p>
      <!-- <div class=""> -->
      <ul class="flex justify-between ">
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
        {
          name: 'contact',
          url: '/get-in-touch'
        },
        {
          name: 'linkedin',
          url: '/get-in-touch'
        },
        {
          name: 'instagram',
          url: '/get-in-touch'
        },
        {
          name: 'twitter',
          url: '/get-in-touch'
        }
      ]
    }
  }
}
</script>

<style></style>
