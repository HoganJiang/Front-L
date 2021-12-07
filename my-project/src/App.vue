<template>
  <div id="app">
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <Hello msg="Welcome to Your Vue.js App" />
    <Hello msg="Welcome to Your Vue.js App" /> -->
    <!-- <Hello msg="Welcome to Your Vue.js App" /> -->
    <!-- <Exercise01 :emotion-happy="emotion" /> -->
    <!-- <Exercise02 :a="fruita" :b="fruitb" :c="fruitc"/> -->
    <Exericse03 @add="sumNum" :msb-value='a' :value-b="b" :value-c="c"></Exericse03>
  </div>
</template>

<script>
// import HelloWorld from "./components/HelloWorld.vue";
// import Hello from "./components/Hello.vue";
// import Exercise01 from "./components/Exercise01.vue"
// import Exercise02 from "./components/Exercise02.vue"
import Exericse03 from "./components/Exercise03.vue"

export default {
  name: "App",
  components: {
    // HelloWorld,
    // Hello,
    // Exercise01,
    // Exercise02,
    Exericse03
  },
  data() {
    return {
      fruita:"apple",
      fruitb:"orange",
      fruitc:"banana",
      a: 100,
      b: 200,
      c: 300
    };
  },
  methods: {
      sumNum(){
        this.a++
      }
  }
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
