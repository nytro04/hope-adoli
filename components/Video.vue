<template>
  <div class="full-width">
    <div class="flex items-center justify-center video">
      <div class="relative">
        <ArrowDownSvg class="" />
        <PlaySvg class="play" />
      </div>
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

.full-width {
  margin-left: -5rem;
  margin-right: -5rem;
}
</style>
