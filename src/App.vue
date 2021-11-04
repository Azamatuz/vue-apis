<template>
    <div id="app">
      <h1>Sport Forcaster</h1>
      <player-view :player="playerView" />
    </div>
</template>

<script>
import PlayerView from './components/PlayerView.vue'


export default {
  components: { PlayerView },
  name: 'App',
  data () {
    return {
      playerView: {
      first_name: "Sidney",
      last_name: "Crosby",
      score: 2
      }


    }
  }

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
