<template>
  <div class="playlist-content-container main-playlist-container">
      <VideoBar v-for="index in 20" :key="index" :videoNumber="index"/>
  </div>
</template>

<script>
import VideoBar from './PlaylistContentVideoBar';
export default {
  name: "PlaylistContent",
  components: { VideoBar }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_main.scss";
button {
  background-color: grey;
  width: 100%;
}

</style>