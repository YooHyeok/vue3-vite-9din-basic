<template>
  <h1>이벤트 핸들링</h1>
  <div>
    <h2>인라인 핸들러</h2>
    <button v-on:click="count++">클릭</button>
    <h3>{{ count }}</h3>
  </div>
  <div>
    <h2>메소드 핸들러</h2>
    <button v-on:click="changeName">클릭</button>
    <h3>{{ name }}</h3>
  </div>
</template>
<script>
export default {
  name: 'VEvent',
  data() {
    return {
      count: 0,
      name: 'Vue.JS'
    }
  },
  methods: {
    changeName() {
      this.name = '변경된 텍스트 데이터 입니다.'
    }
  }
}
</script>