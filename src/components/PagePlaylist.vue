<template>
  <div class="page-playlist-container">
    <aside>
      <AppSidebar/>
    </aside>
    <main>

    </main>
  </div>
</template>

<script>
import AppSidebar from './AppSidebar.vue';

export default {
    name: "PagePlaylist",
    components: { AppSidebar }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
@import "../assets/scss/_main.scss";

div.page-playlist-container, aside {
  height: 100%;
}

@media only screen and (max-width: 790px) {
  aside {
    display: none;
  }
}
</style>

