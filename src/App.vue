<template>
    <div style="height: 100%">
      <PagePlaylist/>
    </div>
</template>

<script>
import PagePlaylist from './components/PagePlaylist.vue'

export default {
  name: 'App',
  components: {
    PagePlaylist,
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

@media screen and (min-width: 1080px){
  html {
    background-color: black;
  }
}
</style>
