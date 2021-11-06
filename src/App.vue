<template>
  <div id="app">
    <h1>Sport Forcaster</h1>
    <player-view :player="playerView" v-if="playerView" />
    <player-list :players="players" :playerView="playerView" />
  </div>
</template>

<script>
import PlayerView from './components/PlayerView.vue'
import PlayerList from './components/PlayerList.vue'

import axios from 'axios'

export default {

  name: 'App',
  data () {
    return {
      playerView: null,
      players: null
    }
  },
  created () {
    axios({
      method: 'get',
      url: 'https://staging.formula.forecaster.ca/api/schedules?season-id=2021&start_date=2021-11-16%2018:59:00&end_date=2021-11-16%2019:01:00'
    })
      .then(responce => (this.players = responce.data))
      .catch(error => console.log(error))
  },
  components: {
    PlayerView,
    PlayerList
  },
  computed: {
    totalRequest () {
      return this.players.reduce((acc, item) => acc + item.player.guessing_score.score, 0)
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
