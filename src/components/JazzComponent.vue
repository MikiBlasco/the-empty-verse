<template>
  <div>
    <img alt="Vue logo" src="../assets/logo.png" class="jazzPic" />
    <h1>{{ msg }}</h1>
  </div>
</template>

<script>
export default {
  name: "JazzComponent",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.jazzPic {
  border-radius: 50%;
  width: 200px;
}
</style>
