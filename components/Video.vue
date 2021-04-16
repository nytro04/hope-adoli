<template>
  <div class="full-width">
    <div class="flex items-center justify-center video">
      <div class="relative">
        <ShowReelSvg class="z-0 show-reel" />
        <PlaySvg class="z-10 play" />
      </div>
    </div>
  </div>
</template>

<script>
import ShowReelSvg from '~/assets/svgs/play-showreel-badge.svg?inline'
import PlaySvg from '~/assets/svgs/play-btn.svg?inline'

export default {
  components: {
    ShowReelSvg,
    PlaySvg
  }
}
</script>

<style lang="scss" scoped>
@import './assets/scss/abstracts/_mixins.scss';

.video {
  background-color: #383838;
  height: 100vh;
  overflow: hidden;

  @include respond(tab-land) {
    height: 25rem;
  }
  @include respond(tab-port) {
    height: 25rem;
  }

  @include respond(phone) {
    height: 14rem;
  }
}

.show-reel {
  @include respond(tab-land) {
    height: 4.875rem;
  }
  @include respond(tab-port) {
    height: 4.875rem;
  }
  @include respond(phone) {
    height: 4.875rem;
  }
}

.play {
  position: absolute;
  top: 5rem;
  left: 5.5rem;
  @include respond(tab-land) {
    height: 1rem;
    position: absolute;
    top: 2rem;
  }
  @include respond(tab-port) {
    height: 1rem;
    position: absolute;
    top: 2rem;
  }
  @include respond(phone) {
    height: 1rem;
    position: absolute;
    top: 2rem;
  }
}

/* .full-width {
  margin-left: -5rem;
  margin-right: -5rem;
} */
</style>
