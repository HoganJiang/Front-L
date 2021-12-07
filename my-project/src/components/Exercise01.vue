<template>
  <div>
    <span>emotion:{{emotionHappy}}</span>
  </div>
</template>

<script>
export default {
  //罗列父组件传进的属性值
  props: ["emotionHappy"],
  data() {
    return {
      emotion: "happy",
    };
  },
  methods:{
      modified(){
        this.emotion = "active"
      }
  }
};
</script>

<style lang="scss" scoped>
</style>