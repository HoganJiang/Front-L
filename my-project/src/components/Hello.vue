<template>
  <div>
    <h3>Welcome to Warm!{{a}}</h3>
    <button @click="add">clik</button>
  </div>
</template>

<script>
  export default {
    data() {
      return {
        a: 1
      };
    },
    methods:{
      add(){
        this.a++
      }
    }
  }
</script>

<style lang="scss" scoped>

</style>