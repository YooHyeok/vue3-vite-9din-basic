<template>
  <h1>[클래스 바인딩 테스트]</h1>
  <h2 v-bind:class="{active: isActive}">isActive: {{ isActive }}</h2>
  <h2 :class="{active: isActive}">isActive: {{ isActive }}</h2>
  <button @click="change">버튼</button>
</template>
<script>
export default {
  name: 'VHtml',
  data() {
    return {
      isActive: false
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