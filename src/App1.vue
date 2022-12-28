<template>
  <div id="app" class="d-flex justify-content-center align-items-center oiai">
    <MusicPlayer />
  </div>
</template>

<script>
import MusicPlayer from './components/MusicPlayer.vue'

export default {
  name: 'app',
  components: {
    MusicPlayer
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css?family=Source+Code+Pro&display=swap');

#app {
  font-family: 'Source Code Pro', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  height: 100vh;
  color: #264b65;
  background: #fffaf0;
}
</style>
