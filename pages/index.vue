<template>
  <!-- <div class="relative"> -->
  <div class="overflow-hidden">
    <LandingPage />
    <div class="my-64"></div>
    <Video />
    <div class="my-64"></div>
    <RecentWorks />
    <div class=" my-80"></div>

    <Jobs />

    <div class="mt-80"></div>
    <Links />
    <div class="my-40"></div>
    <!-- <Footer /> -->
  </div>
</template>

<script>
export default {
  components: {
    LandingPage: () => import('~/components/LandingPage'),
    Video: () => import('~/components/Video'),
    RecentWorks: () => import('~/components/RecentWorks'),
    Links: () => import('~/components/Links'),
    Jobs: () => import('~/components/Jobs')
  },
  head() {
    return {
      title: 'Hope Adoli | Portfolio Index'
    }
  }
}
</script>

<style scoped lang="scss"></style>
