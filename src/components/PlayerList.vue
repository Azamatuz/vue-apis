<template>
    <div  v-for="(player, index) in players" :key="index">
        <p>{{player.player-name}}</p>        
    </div>
</template>

<script>
    export default {
        name: 'player-list',
        props: ['players', 'playerView']
    }
</script>

