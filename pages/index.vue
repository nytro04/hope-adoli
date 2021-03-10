<template>
  <div class="container mx-auto">
    <LandingPage />
    <div class="my-64"></div>
    <Video />
  </div>
</template>

<script>
export default {
  components: {
    LandingPage: () => import('~/components/LandingPage'),
    Video: () => import('~/components/Video')
  },
  head() {
    return {
      title: 'Hope Adoli | Portfolio Index'
    }
  }
}
</script>

<style scoped lang="scss">
// img {
//   width: 100%;
//   height: auto;
// }
// .container {
//   background: #000;
//   display: grid;
//   grid-template-columns: repeat(2, 1fr);
//   gap: 1em;
//   // grid-template-rows: repeat(6, 1fr);
//   grid-template-rows: auto 1fr 1fr 3fr 1fr 1fr;
// }

// .title {
//   grid-column: span 2;
// }

// .team-member {
//   border: 2px solid white;
//   background-color: black;
//   text-align: center;
// }

// .member-1 {
//   grid-row-start: 2;
//   grid-column-start: 2;
//   grid-row-end: 5;
// }
// .member-2 {
//   grid-row-start: 3;
//   grid-column-start: 1;
//   grid-row-end: 5;
// }
// .member-1 {
//   grid-row-start: 3;
//   grid-column-start: 1;
//   grid-row-end: 5;
// }
// .member-2 {
//   grid-row-start: 2;
//   grid-column-start: 2;
//   grid-row-end: 5;
// }
// .member-3 {
//   grid-row-start: 4;
//   grid-column-start: 3;
//   grid-row-end: 7;
// }
</style>
