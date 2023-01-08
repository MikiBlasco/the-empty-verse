<template>
  <div class="secondComponent">
    <button v-on:click="show()">Jazz</button>
    <div v-if="showInfo" class="list">
      <h1>{{ msg }}</h1>
      <!-- <div v-for="item in arrayProp" :key="item">
        {{ item }}
      </div> -->
      <a href="https://mikiblasco.github.io/Jazz-Wine-Canvas-Game/">
        <button>Play!</button>
      </a>
    </div>
  </div>
</template>

<script lang="js">

  export default  {
    name: 'SecondComponent',
    props: {
    msg: String,
    },
    mounted () {
    },
    data () {
      return {
        arrayProp: ["The", "empty", "verse"],
        showInfo: false
      }
    },
    methods: {
      show(){
        if (this.showInfo === true) {
          console.log("was true and now false", this.showInfo)
         return this.showInfo = false
        } else {
          console.log("was false and now true", this.showInfo)
          return this.showInfo = true
        }
      }
    },
    computed: {

    }
}
</script>

<style scoped>
.list {
  margin: 10px;
}
div > button {
  margin: 10px;
  padding: 5px;
  background-color: rgb(149, 152, 234);
  color: rgb(59, 1, 1);
  border: 1px solid rgb(90, 4, 4);
  font-weight: bold;
}
a > button {
  margin: 10px;
  padding: 5px;
  background-color: rgb(244, 154, 154);
  color: rgb(26, 1, 55);
  font-weight: bold;
}
</style>
