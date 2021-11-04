<template>
    <div id="app">
      <h1>Sport Forcaster</h1>
      <player-view :player="playerView" 
      v-if="playerView"
      />
      <player-list
      :players="players"
      :playerView="playerView"
      />
    </div>
</template>

<script>
import PlayerView from './components/PlayerView.vue';
import PlayerList from './components/PlayerList.vue';


export default {

  name: 'App',
  data () {
    return {
      playerView: null,
      players: [
        {
"player-key": 26068,
"player-name": "Brett Murray",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 1, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 3, \"orig-games-played-home\": 0, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 20931,
"player-name": "Christian Wolanin",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 1, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 10, \"orig-games-played-home\": 8, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 12293,
"player-name": "Craig Anderson",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 20, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 0, \"orig-games-played-home\": 0, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 13952,
"player-name": "Sabres Buffalo",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 0, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 0, \"orig-games-played-home\": 0, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 15725,
"player-name": "Kyle Okposo",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 3, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 2, \"predicted-assists-season\": 16, \"predicted-games-played-season\": 57, \"predicted-goals-season\": 7}",
"score": "0.0684932"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 19, \"orig-games-played-home\": 24, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 3, \"predicted-goals-season\": 7, \"scaling-factor\": 0.9508995, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 2}",
"scaling_factor": 0.9508995,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 2, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 7, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 2, \"percentage\": 0, \"predicted-goals-season\": 7, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 2, \"percentage\": 1, \"predicted-goals-season\": 7, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0706355,
"scaling_factor": 1.0312777985656498,
"boost": 3.13,
"average_score": 0.0684932
}
},
{
"player-key": 16031,
"player-name": "Dustin Tokarski",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 1, \"predicted-games-played-season\": 1, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 0, \"orig-games-played-home\": 0, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 17455,
"player-name": "Cody Eakin",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 1, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 11, \"predicted-games-played-season\": 79, \"predicted-goals-season\": 11}",
"score": "0.1369863"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 22, \"orig-games-played-home\": 27, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 3, \"predicted-goals-season\": 11, \"scaling-factor\": 0.9509002, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 1}",
"scaling_factor": 0.9509002,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 11, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 11, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 11, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.141271,
"scaling_factor": 1.03127855773574,
"boost": 3.13,
"average_score": 0.1369863
}
},
{
"player-key": 17896,
"player-name": "Jeff Skinner",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 2, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 17, \"predicted-games-played-season\": 78, \"predicted-goals-season\": 17}",
"score": "0.2191781"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 29, \"orig-games-played-home\": 32, \"orig-goals-scored-away\": 6, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 17, \"scaling-factor\": 0.9508998, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 1}",
"scaling_factor": 0.9508998,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 17, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 17, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 17, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.2260336,
"scaling_factor": 1.0312781239242599,
"boost": 3.13,
"average_score": 0.2191781
}
},
{
"player-key": 17919,
"player-name": "Mark Pysyk",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 1, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 8, \"predicted-games-played-season\": 75, \"predicted-goals-season\": 4}",
"score": "0.0547945"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 22, \"orig-games-played-home\": 22, \"orig-goals-scored-away\": 2, \"orig-goals-scored-home\": 1, \"predicted-goals-season\": 4, \"scaling-factor\": 0.9508998, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9508998,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 4, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 4, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 4, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0565084,
"scaling_factor": 1.0312781239242599,
"boost": 3.13,
"average_score": 0.0547945
}
},
{
"player-key": 19220,
"player-name": "Colin Miller",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 5, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 9, \"predicted-games-played-season\": 57, \"predicted-goals-season\": 3}",
"score": "0.0410959"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 27, \"orig-games-played-home\": 29, \"orig-goals-scored-away\": 4, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 3, \"scaling-factor\": 0.9509004, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9509004,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 3, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 3, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 3, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0423813,
"scaling_factor": 1.03127877464148,
"boost": 3.13,
"average_score": 0.0410959
}
},
{
"player-key": 19312,
"player-name": "Drake Caggiula",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 1, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 8, \"predicted-games-played-season\": 51, \"predicted-goals-season\": 3}",
"score": "0.0273973"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 21, \"orig-games-played-home\": 25, \"orig-goals-scored-away\": 2, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 3, \"scaling-factor\": 0.9509017, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 1}",
"scaling_factor": 0.9509017,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 3, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 3, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 3, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0282543,
"scaling_factor": 1.0312801845287898,
"boost": 3.13,
"average_score": 0.0273973
}
},
{
"player-key": 19356,
"player-name": "Zemgus Girgensons",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 3, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 3, \"predicted-assists-season\": 11, \"predicted-games-played-season\": 68, \"predicted-goals-season\": 10}",
"score": "0.0958904"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 3, \"orig-games-played-home\": 5, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 10, \"scaling-factor\": 0.9509001, \"season-goals-scored-away\": 1, \"season-goals-scored-home\": 2}",
"scaling_factor": 0.9509001,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 3, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 10, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 3, \"percentage\": 0, \"predicted-goals-season\": 10, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 3, \"percentage\": 1, \"predicted-goals-season\": 10, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0988897,
"scaling_factor": 1.03127844928287,
"boost": 3.13,
"average_score": 0.0958904
}
},
{
"player-key": 19603,
"player-name": "Vinnie Hinostroza",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 2, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 12, \"predicted-games-played-season\": 70, \"predicted-goals-season\": 9}",
"score": "0.109589"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 16, \"orig-games-played-home\": 18, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 5, \"predicted-goals-season\": 9, \"scaling-factor\": 0.9508998, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 1}",
"scaling_factor": 0.9508998,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 9, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 9, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 9, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.1130167,
"scaling_factor": 1.0312781239242599,
"boost": 3.13,
"average_score": 0.109589
}
},
{
"player-key": 19863,
"player-name": "Jack Eichel",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 40, \"predicted-games-played-season\": 77, \"predicted-goals-season\": 26}",
"score": "0.3561644"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 12, \"orig-games-played-home\": 9, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 26, \"scaling-factor\": 0.9509, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9509,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 26, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 26, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 26, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.3673046,
"scaling_factor": 1.03127834083,
"boost": 3.13,
"average_score": 0.3561644
}
},
{
"player-key": 20122,
"player-name": "Will Butcher",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 1, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 15, \"predicted-games-played-season\": 62, \"predicted-goals-season\": 5}",
"score": "0.0684932"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 14, \"orig-games-played-home\": 16, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 5, \"scaling-factor\": 0.9508995, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9508995,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 5, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 5, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 5, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0706355,
"scaling_factor": 1.0312777985656498,
"boost": 3.13,
"average_score": 0.0684932
}
},
{
"player-key": 20193,
"player-name": "Robert Hagg",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 1, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 1, \"predicted-goals-season\": 0}",
"score": "-0.0136986"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 20, \"orig-games-played-home\": 22, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 1}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": -0.0136986
}
},
{
"player-key": 20202,
"player-name": "John Hayden",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 1, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 17, \"orig-games-played-home\": 16, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 20800,
"player-name": "Anders Bjork",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 1, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 14, \"predicted-games-played-season\": 80, \"predicted-goals-season\": 14}",
"score": "0.1780822"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 25, \"orig-games-played-home\": 28, \"orig-goals-scored-away\": 2, \"orig-goals-scored-home\": 4, \"predicted-goals-season\": 14, \"scaling-factor\": 0.9508997, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 1}",
"scaling_factor": 0.9508997,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 14, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 14, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 14, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.1836523,
"scaling_factor": 1.0312780154713899,
"boost": 3.13,
"average_score": 0.1780822
}
},
{
"player-key": 20957,
"player-name": "Victor Olofsson",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 4, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 5, \"predicted-assists-season\": 28, \"predicted-games-played-season\": 79, \"predicted-goals-season\": 19}",
"score": "0.1917808"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 31, \"orig-games-played-home\": 33, \"orig-goals-scored-away\": 8, \"orig-goals-scored-home\": 10, \"predicted-goals-season\": 19, \"scaling-factor\": 0.9208715, \"season-goals-scored-away\": 1, \"season-goals-scored-home\": 4}",
"scaling_factor": 0.9208715,
"boost": -7.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 5, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 19, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 5, \"percentage\": 0, \"predicted-goals-season\": 19, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 5, \"percentage\": 1, \"predicted-goals-season\": 19, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.1915337,
"scaling_factor": 0.9987115707620499,
"boost": -0.13,
"average_score": 0.1917808
}
},
{
"player-key": 21735,
"player-name": "Andrew Oglevie",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 1, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 0, \"orig-games-played-home\": 0, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
},
{
"player-key": 21785,
"player-name": "Rasmus Dahlin",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 4, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 35, \"predicted-games-played-season\": 82, \"predicted-goals-season\": 7}",
"score": "0.0958904"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 31, \"orig-games-played-home\": 33, \"orig-goals-scored-away\": 3, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 7, \"scaling-factor\": 0.9509001, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9509001,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 7, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 7, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 7, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0988897,
"scaling_factor": 1.03127844928287,
"boost": 3.13,
"average_score": 0.0958904
}
},
{
"player-key": 25970,
"player-name": "Tage Thompson",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 2, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 2, \"predicted-assists-season\": 12, \"predicted-games-played-season\": 69, \"predicted-goals-season\": 12}",
"score": "0.1369863"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 18, \"orig-games-played-home\": 28, \"orig-goals-scored-away\": 2, \"orig-goals-scored-home\": 8, \"predicted-goals-season\": 12, \"scaling-factor\": 0.9509002, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 2}",
"scaling_factor": 0.9509002,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 2, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 12, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 2, \"percentage\": 0, \"predicted-goals-season\": 12, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 2, \"percentage\": 1, \"predicted-goals-season\": 12, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.141271,
"scaling_factor": 1.03127855773574,
"boost": 3.13,
"average_score": 0.1369863
}
},
{
"player-key": 25984,
"player-name": "Rasmus Asplund",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 2, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 4, \"predicted-assists-season\": 20, \"predicted-games-played-season\": 78, \"predicted-goals-season\": 20}",
"score": "0.2191781"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 17, \"orig-games-played-home\": 19, \"orig-goals-scored-away\": 7, \"orig-goals-scored-home\": 4, \"predicted-goals-season\": 20, \"scaling-factor\": 0.9508998, \"season-goals-scored-away\": 3, \"season-goals-scored-home\": 1}",
"scaling_factor": 0.9508998,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 4, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 20, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 4, \"percentage\": 0, \"predicted-goals-season\": 20, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 4, \"percentage\": 1, \"predicted-goals-season\": 20, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.2260336,
"scaling_factor": 1.0312781239242599,
"boost": 3.13,
"average_score": 0.2191781
}
},
{
"player-key": 26332,
"player-name": "Arttu Ruotsalainen",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 20, \"predicted-games-played-season\": 77, \"predicted-goals-season\": 23}",
"score": "0.3013699"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 12, \"orig-games-played-home\": 12, \"orig-goals-scored-away\": 3, \"orig-goals-scored-home\": 3, \"predicted-goals-season\": 23, \"scaling-factor\": 0.9509, \"season-goals-scored-away\": 1, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9509,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 23, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 23, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 23, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.3107963,
"scaling_factor": 1.03127834083,
"boost": 3.13,
"average_score": 0.3013699
}
},
{
"player-key": 26493,
"player-name": "Jacob Bryson",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 4, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 14, \"predicted-games-played-season\": 74, \"predicted-goals-season\": 4}",
"score": "0.0547945"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 23, \"orig-games-played-home\": 23, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 4, \"scaling-factor\": 0.9508998, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9508998,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 4, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 4, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 4, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0565084,
"scaling_factor": 1.0312781239242599,
"boost": 3.13,
"average_score": 0.0547945
}
},
{
"player-key": 26524,
"player-name": "Henri Jokiharju",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 15, \"predicted-games-played-season\": 80, \"predicted-goals-season\": 6}",
"score": "0.0821918"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 25, \"orig-games-played-home\": 22, \"orig-goals-scored-away\": 1, \"orig-goals-scored-home\": 2, \"predicted-goals-season\": 6, \"scaling-factor\": 0.9509004, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9509004,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 6, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 6, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 6, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.0847627,
"scaling_factor": 1.03127877464148,
"boost": 3.13,
"average_score": 0.0821918
}
},
{
"player-key": 26613,
"player-name": "Casey Mittelstadt",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 18, \"predicted-games-played-season\": 76, \"predicted-goals-season\": 15}",
"score": "0.2054795"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 20, \"orig-games-played-home\": 22, \"orig-goals-scored-away\": 4, \"orig-goals-scored-home\": 6, \"predicted-goals-season\": 15, \"scaling-factor\": 0.9508999, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9508999,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 15, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 15, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 15, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.2119065,
"scaling_factor": 1.03127823237713,
"boost": 3.13,
"average_score": 0.2054795
}
},
{
"player-key": 27213,
"player-name": "Mattias Samuelsson",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 12, \"predicted-games-played-season\": 67, \"predicted-goals-season\": 1}",
"score": "0.0136986"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 6, \"orig-games-played-home\": 6, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 1, \"scaling-factor\": 0.950898, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.950898,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 1, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 1, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 1, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.014127,
"scaling_factor": 1.0312761717726,
"boost": 3.13,
"average_score": 0.0136986
}
},
{
"player-key": 27450,
"player-name": "Dylan Cozens",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 2, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 1, \"predicted-assists-season\": 23, \"predicted-games-played-season\": 80, \"predicted-goals-season\": 16}",
"score": "0.2054795"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 27, \"orig-games-played-home\": 22, \"orig-goals-scored-away\": 4, \"orig-goals-scored-home\": 1, \"predicted-goals-season\": 16, \"scaling-factor\": 0.9508999, \"season-goals-scored-away\": 1, \"season-goals-scored-home\": 0}",
"scaling_factor": 0.9508999,
"boost": -4.91
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 16, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 0, \"predicted-goals-season\": 16, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 1, \"percentage\": 1, \"predicted-goals-season\": 16, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0.2119065,
"scaling_factor": 1.03127823237713,
"boost": 3.13,
"average_score": 0.2054795
}
},
{
"player-key": 28098,
"player-name": "Lukas Rousek",
"actual-score": "--",
"algorithms": {
"average": {
"intermediate_values": "{\"actual-assists\": 0, \"actual-games-played\": 9, \"games-left\": 73, \"goals-scored\": 0, \"predicted-assists-season\": 0, \"predicted-games-played-season\": 0, \"predicted-goals-season\": 0}",
"score": "0"
},
"home-away-weighting": {
"intermediate_values": "{\"game-house\": \"away\", \"games-left-away\": 37, \"games-left-home\": 36, \"orig-games-played-away\": 0, \"orig-games-played-home\": 0, \"orig-goals-scored-away\": 0, \"orig-goals-scored-home\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 0, \"season-goals-scored-away\": 0, \"season-goals-scored-home\": 0}",
"scaling_factor": 0,
"boost": -100
},
"goals-against-average": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"opponent-gaa\": 2.9, \"predicted-goals-season\": 0, \"scaling-factor\": 1.0845287, \"upcoming-opponents-gaa\": 2.6739726}",
"scaling_factor": 1.0845287,
"boost": 8.45
},
"x-factor": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 0, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"x-factor-reason\": null}",
"scaling_factor": 1,
"boost": 0
},
"schedule": {
"intermediate_values": "{\"games-left\": 73, \"goals-scored\": 0, \"percentage\": 1, \"predicted-goals-season\": 0, \"scaling-factor\": 1, \"schedule-situation\": null}",
"scaling_factor": 1,
"boost": 0
}
},
"guessing-score": {
"score": 0,
"scaling_factor": 0,
"boost": -100,
"average_score": 0
}
}

      ]
      };


    },
      components: {PlayerView, PlayerList},
  };


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
