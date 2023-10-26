<template>
  <favorite-panel :cards-list-data="favoriteSources" />
</template>

<script>
import FavoritePanel from './components/FavoritePanel.vue'
import { favoriteSources } from './constants/1_data_google_favorite'

export default {
  name: 'App',

  components: {
    FavoritePanel,
  },

  data() {
    return {
      favoriteSources,
    }
  },
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
