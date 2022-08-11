<script setup>
import Inputs from "./Inputs.vue";
import Buttons from "./Buttons.vue";
</script>

<template>
  <div class="neon-wrapper">
    <h1 class="neon-text">Neon Retro</h1>

    <div class="body">
      <h2 class="neon-text">Buttons</h2>
      <Buttons />
    </div>
    <div class="body">
      <h2 class="neon-text">Inputs</h2>
      <Inputs />
    </div>
  </div>
</template>

<style scoped>
@import url(https://fonts.googleapis.com/css?family=Mr+Dafoe);
@import url(https://fonts.googleapis.com/css?family=Titillium+Web:900);
@import url(https://fonts.googleapis.com/css?family=Righteous);
@import url(https://fonts.googleapis.com/css?family=Candal);
@import url(https://fonts.googleapis.com/css?family=Permanent+Marker);
@import url(https://fonts.googleapis.com/css?family=Monoton);
@import url(https://fonts.googleapis.com/css?family=Sacramento:400);

body {
  font-size: 18px;
  display: flex;
  justify-content: center;
  align-items: center;
}
h1 {
  font-family: "Sacramento", sans-serif;
  font-size: 5.2rem;
  animation: pulsate 1.5s infinite alternate;
  border: 0.2rem solid #fff;
  border-radius: 2rem;
  padding: 0.4em;
  width: 55rem;
  margin: auto;
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #bc13fe,
    0 0 0.8rem #bc13fe, 0 0 2.8rem #bc13fe, inset 0 0 1.3rem #bc13fe;
}
h2 {
  font-size: 3.2rem;
  margin-bottom: 0;
}

.buttons {
  margin-bottom: 2rem;
}

.neon-text {
  color: #fff;
  font-family: "Sacramento", sans-serif;
  text-shadow: 0 0 7px #fff, 0 0 10px #fff, 0 0 21px #fff, 0 0 42px #bc13fe,
    0 0 82px #bc13fe, 0 0 92px #bc13fe, 0 0 102px #bc13fe, 0 0 151px #bc13fe;
}
.body {
  width: 50rem;
  margin: auto;
  background-color: rgba(30, 27, 29, 0.8);
  box-shadow: 0 0 0.2rem #fff, 0 0 0.2rem #fff, 0 0 2rem #13a8fe,
    0 0 0.8rem #13a8fe, 0 0 2.8rem #13a8fe, inset 0 0 1.3rem #13a8fe;
}

@keyframes pulsate {
  100% {
    text-shadow: 0 0 4px #fff, 0 0 11px #fff, 0 0 19px #fff, 0 0 40px #bc13fe,
      0 0 80px #bc13fe, 0 0 90px #bc13fe, 0 0 100px #bc13fe, 0 0 150px #bc13fe;
  }

  0% {
    text-shadow: 0 0 2px #fff, 0 0 4px #fff, 0 0 6px #fff, 0 0 10px #bc13fe,
      0 0 45px #bc13fe, 0 0 55px #bc13fe, 0 0 70px #bc13fe, 0 0 80px #bc13fe;
  }
}
</style>