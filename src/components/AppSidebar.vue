<template>
  <aside>
    <AppSidebarButton title="Home">
      <template #icon>
        <i class="fa-solid fa-house"></i>
      </template>
    </AppSidebarButton>
  </aside>
</template>

<script>
import AppSidebarButton from './AppSidebarButton.vue';

export default {
  name: "AppSidebar",
  components: { AppSidebarButton },
  data() {
    
  }
}
</script>

<style scoped lang="scss">
@import "../assets/scss/_main.scss";

aside {
  width: $sidebar-width;
  height: 100vw;
  background-color: $base-dark-bg;
  padding: 0 4px;
}

</style>