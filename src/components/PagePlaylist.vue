<template>
  <div class="page-playlist-container">
    <aside>
      <AppSidebar/>
    </aside>

    <main>
      <PlaylistHeader class="main--playlist-header"/>
      <PlaylistContent class="main--playlist-content"/>
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
  margin-left: $sidebar-width;
}

.main--playlist-header {
  background: linear-gradient(to bottom, rgba(101, 104, 164, 0.800) 0%, rgba(48, 39, 52,0.298) 33.000001%, rgba(15,15,15,1.000) 100%);
}

.main--playlist-content {
  background-color: $base-dark-bg;
  flex-grow: 1;
  padding: 0px 24px;
}

@media only screen and (max-width: 790px) {
  aside {
    display: none;
  }

  main {
    margin-left: 0;
  }
}

@media screen and (min-width: 1080px){
  main {
    flex-direction: row;
  } 

  div.main--playlist-content {
    margin-left: 400px;
    margin-top: 40px;
  }
  
}
</style>

