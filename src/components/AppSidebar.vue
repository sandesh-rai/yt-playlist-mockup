<template>
  <div class="side-bar-container">
    <AppSidebarButton v-for="button in sidebarButtons" :title="button.title" :key="button.id">
      <template #icon>
        <i :class="button.icon"></i>
      </template>
    </AppSidebarButton>
  </div>
</template>

<script>
import AppSidebarButton from './AppSidebarButton.vue';

export default {
  name: "AppSidebar",
  components: { AppSidebarButton },
  data() {
    return {
      sidebarButtons: [
      {
        id: 1,
        icon: "fa-solid fa-house",
        title: "Home"
      },
      {
        id: 2,
        icon: "fa-solid fa-file-video",
        title: "Shorts"
      },
      {
        id: 3,
        icon: "fa-solid fa-clapperboard",
        title: "Subscriptions"
      },
      {
        id: 4,
        icon: "fa-solid fa-film",
        title: "Library"
      },
    ]
    };
  }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_main.scss";

div.side-bar-container {
  position: fixed;
  width: $sidebar-width;
  height: 100%;
  background-color: $base-dark-bg;
  padding: 4px;
}
</style>