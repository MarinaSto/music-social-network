<template>
    <div class="bg-green-500 rounded">
        <div id="aplayer"></div>
    </div>
</template>
<script setup>
import { onMounted } from 'vue'
import APlayer from 'aplayer'
import 'aplayer/dist/APlayer.min.css';
onMounted(() => {
    thePlayer();
})
const thePlayer = () => {
    new APlayer({
        container: document.getElementById('aplayer'),
        audio: [{
            name: 'First song',
            artist: 'artist',
            url: '/music/europe-travel.mp3',
            cover: 'cover.jpg',
        }]
    })
}
</script>