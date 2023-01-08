<template>
  <div id="app">
    <JazzComponent msg="Welcome to the Jazz Empty Verse" />
    <SecondComponent />
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
  props: {
    arrayApp: [],
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
