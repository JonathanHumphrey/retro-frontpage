<template>
  <HelloWorld />
  <NeonRetro />
</template>

<script>
import NeonRetro from "./components/NeonRetro.vue";
import HelloWorld from "./components/HelloWorld.vue";

export default {
  name: "App",
  components: {
    NeonRetro,
    HelloWorld,
  },
};
</script>

<style>
#app {
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
