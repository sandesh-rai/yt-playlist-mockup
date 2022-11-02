<template>
  <div class="page-playlist-container">
    <aside>
      <AppSidebar/>
    </aside>

    <main>
      <PlaylistHeader/>
      <PlaylistContent class="playlist-content"/>
    </main>
  </div>
</template>

<script>
import AppSidebar from './AppSidebar.vue';
import PlaylistHeader from './PlaylistHeader.vue';
import PlaylistContent from './PlaylistContent.vue';

export default {
    name: "PagePlaylist",
    components: { AppSidebar, PlaylistHeader, PlaylistContent }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/_main.scss";

div.page-playlist-container, aside {
  height: 100%;
  display: flex;
}

main {
  display: flex;
  flex-direction: column;
  flex-grow: 1;
}

.playlist-content {
  flex-grow: 1;
}

@media only screen and (max-width: 790px) {
  aside {
    display: none;
  }
}
</style>

