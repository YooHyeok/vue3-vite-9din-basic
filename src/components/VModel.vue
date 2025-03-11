<template>
  <h1>[Vue.js v-model]</h1>
  <div>
    <input type="text" v-model="inputValue1">
    <input type="text" @input="inputValue2 = $event.value.target">
  </div>
  <div>v-model: {{ inputValue1 }}</div>
  <div>@input: {{ inputValue2 }}</div>
</template>
<script>
export default {
  data() {
    return {
      inputValue1: '',
      inputValue2: ''
    }
  }
}
</script>