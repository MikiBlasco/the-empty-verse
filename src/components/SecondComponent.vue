<template>
  <div class="secondComponent">
    <button v-on:click="show()">Jazz</button>
    <div v-if="showInfo" class="list">
      <div v-for="item in arrayProp" :key="item">
        {{ item }}
      </div>
      <a href="https://mikiblasco.github.io/Jazz-Wine-Canvas-Game/">
        <button>Play!</button>
      </a>
    </div>
  </div>
</template>

<script lang="js">

  export default  {
    name: 'SecondComponent',
    props: [],
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
</style>
