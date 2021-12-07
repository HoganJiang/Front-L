<template>
  <div>
    <h1>
      马士兵教育，我接收到的父组件的值是：{{ msbValue }} {{ valueB }}
      {{ valueC }}
    </h1>
    <button @click="add">按我加1</button>
  </div>
</template>
<script>
export default {
  // 罗列父组件传进的属性值
  props: {
    msbValue: Number,
    valueB: Number,
    valueC: Number,
  },
  data() {
    return {};
  },
  methods: {
    add() {
      this.$emit("add");
    },
  },
};
</script>
<style>
</style>