<template>
  <div>{{ count }}</div>
</template>

<script>
export default {
  name: 'App',

  data() {
    return {
      count: 0
    };
  },
  beforeCreate() {
    console.log("LifeCycle is beforeCrete", this.count) //  컴포넌트가 생성되기 전 이므로 undefined 출력
  },
  created() {
    console.log("LifeCycle is creted", this.count) // 컴포넌트가 생성된 후 초기화 진행되므로 0 출력
  }
};
</script>

<style scoped></style>