<template>
  <div class="flex items-center justify-center video">
    <div class="relative">
      <ArrowDownSvg class="" />
      <PlaySvg class="play" />
    </div>
  </div>
</template>

<script>
import ArrowDownSvg from '~/assets/svgs/play-showreel-badge.svg?inline'
import PlaySvg from '~/assets/svgs/play-btn.svg?inline'

export default {
  components: {
    ArrowDownSvg,
    PlaySvg
  }
}
</script>

<style lang="scss" scoped>
.video {
  background-color: #383838;
  height: 100vh;
}

.play {
  position: absolute;
  top: 5rem;
  left: 5.5rem;
}
</style>
