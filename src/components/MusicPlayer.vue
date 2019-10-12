<template>
  <div class="music-player w-100 d-flex flex-column border bg-white">
    <div class="music-player__header">

    </div>
    <div class="music-player__main p-4">
      <h5 class="music-player__title">When you look me in the eyes</h5>
      <p class="music-player__singer">Jonas Brother</p>
      <div class="music-player__control mt-5 d-flex">
        <div class="music-player__btn d-flex align-items-center">
          <font-awesome-icon :icon="['fas', 'backward']" />
        </div>
        <div class="music-player__btn play mx-4">
          <font-awesome-icon :icon="['fas', 'play-circle']" />
        </div>
        <div class="music-player__btn d-flex align-items-center">
          <font-awesome-icon :icon="['fas', 'forward']" />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MusicPlayer',
  props: {
    msg: String
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="sass" scoped>
.music-player
  max-width: 500px
  border-radius: 8px
  overflow: hidden
  box-shadow: 0 0 2em rgba(53,89,135,0.2)

  &__header
    height: 200px
    background: url(https://images.pexels.com/photos/92080/pexels-photo-92080.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260) no-repeat
    background-size: cover
    background-position: center

  &__title
    font-weight: 600
    width: 80%

  &__btn
    font-size: 2em
    cursor: pointer

    &.play
      font-size: 2.3em
</style>
