<template>
  <div id="app">
    <JazzComponent />
    <SecondComponent msg="Welcome to the JAZZ VERSE bitch!" />
  </div>
</template>

<script>
import JazzComponent from "./components/JazzComponent.vue";
import SecondComponent from "./components/SecondComponent.vue";
export default {
  name: "App",
  components: {
    JazzComponent,
    SecondComponent,
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
}
</style>
