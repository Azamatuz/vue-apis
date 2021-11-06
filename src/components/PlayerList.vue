<template>
  <div>
    <table class="table">
  <thead>
    <tr>
      <th scope="col">#</th>
      <th scope="col">Name</th>
      <th scope="col">Boost</th>
      <th scope="col">Score</th>
      <th scope="col">Score Sum</th>
    </tr>
  </thead>
  <tbody>
    <tr v-for="(player, index) in players" :key="index">
      <th scope="row" >{{ index }}</th>
      <td>{{player.away-team.players.player-name}}</td>
      <td>{{player.guessing_score.boost}}</td>
      <td>{{player.guessing_score.score}}</td>
      <td>{{ player.id }}</td>

    </tr>

  </tbody>
</table>
{{ players }}
    </div>

</template>

<script>
export default {
  sum: 10,
  name: 'player-list',
  props: ['players', 'playerView', 'totalRequest']
}
</script>
