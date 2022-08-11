<template>
  <div class="music-wrapper">
    <audio id="myAudio" controls autoplay loop>
      <source src="../assets/music.mp3" type="audio/mp3" />
      <code>audio</code> element.
    </audio>
  </div>
</template>

<script setup>
import { onMounted } from "vue";
onMounted(() => {
  var audio = document.getElementById("myAudio");
  audio.volume = 0.05;
});
</script>
<style scoped>
.music-wrapper {
  position: sticky;
  border: solid black;
  width: 20rem;
}
</style>