<template>
  <div class="music-player w-100 d-flex flex-column border bg-white">
    <div class="header"></div>
    <div class="main p-4">
      <h5 class="title">When you look me in the eyes</h5>
      <p class="singer">Jonas Brother</p>
      <div class="audio">
        <audio class="w-100" controls>
          <source src="../assets/when-you-look-me-in-the-eyes.mp3" type="audio/mp3">
          Your browser does not support the audio
        </audio>
      </div>
      <div class="control mt-5 d-none">
        <div class="btn d-flex align-items-center">
          <font-awesome-icon :icon="['fas', 'backward']" />
        </div>
        <div class="btn play">
          <font-awesome-icon :icon="['fas', 'play-circle']" />
        </div>
        <div class="btn d-flex align-items-center">
          <font-awesome-icon :icon="['fas', 'forward']" />
        </div>
      </div>
    </div>a
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

  .main
    padding: 38px

  .header
    height: 200px
    background: url(https://images.pexels.com/photos/92080/pexels-photo-92080.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=750&w=1260) no-repeat
    background-size: cover
    background-position: center

  .title
    font-weight: 600

  .btn
    font-size: 2em
    cursor: pointer

    &.play
      font-size: 2.3em
</style>
