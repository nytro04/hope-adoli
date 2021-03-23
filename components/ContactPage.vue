<template>
  <div class="container mx-auto text-black bg-white contact">
    <div class="sidenav">
      <div>
        <i
          class="cursor-pointer hover:bg-black hover:text-white closebtn"
          @click="close()"
        >
          &times;
        </i>
      </div>
      <div class="flex">
        <h1 class="heading heading__primary">
          GrainMate <br />
          mobile app
        </h1>
        <p>
          Thanks in advance for reaching out! Please note that the contact form
          is for work only. If you just want to say hello, then hit me up on any
          of my social media handles.
        </p>
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
