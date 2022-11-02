<template>
    <div style="height: 100%">
      <AppNavbar/>
      <PagePlaylist/>
    </div>
</template>

<script>
import PagePlaylist from './components/PagePlaylist.vue'
import AppNavbar from './components/AppNavbar.vue'

export default {
  name: 'App',
  components: {
    PagePlaylist,
    AppNavbar
  }
}
</script>

<style>
html {
  height: 100%;
  font-size: 10px;
  font-family: Roboto, Arial, sans-serif;
}

body {
  margin: 0;
  padding: 0;
  height: 100%;
}
</style>
