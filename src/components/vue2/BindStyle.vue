<template>
  <h1>[스타일 바인딩 테스트]</h1>
  <h3 style="color: red; font-size: 24px">인라인스타일 바인딩</h3>
  <h3 :style="{color: '#888888', fontSize: 48 + 'px'}">Vue.JS스타일 바인딩</h3>
  <h3 :style="{color: fontColor, fontSize: fontSize + 'px'}">Vue.JS스타일 바인딩 - 변수활용</h3>
</template>
<script>
export default {
  name: 'BindStyle',
  data() {
    return {
      fontColor: '#999999',
      fontSize: 36
    }
  },
  methods: {
    change() {
      this.isActive = !this.isActive;
    }
  }
}
</script>
<style scoped>
h2.active {
  color: green;
}
</style>