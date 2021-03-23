<template>
  <div class="container mx-auto text-black bg-white contact">
    <div class="px-20 pt-20 pb-10 sidenav">
      <i
        class="cursor-pointer hover:bg-black hover:text-white closebtn"
        @click="close()"
      >
        &times;
      </i>

      <div class="flex">
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
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    close() {
      this.$emit('close-slide')
    }
  }
}
</script>

<style></style>
