<template>
  <div
    class="container h-auto px-10 py-8 mx-auto overflow-y-auto text-center text-black bg-white contact"
  >
    <h3 class="mb-5 font-semibold text-center">
      Hi 👋🙈
    </h3>
    <h3 class="text-center ">
      Thank you for visiting my portfolio website, Please note that it is
      currently under contruction so I'd like to apologize in advance for any
      inconvenience you may have to deal with. Thank you. 😊
    </h3>

    <button class="mt-10 btn btn__black" @click="close">
      Yes, I understand
    </button>
  </div>
</template>

<script>
export default {
  props: {
    close: {
      type: Function,
      default: () => ({})
    }
  }
}
</script>

<style lang="scss" scoped></style>
