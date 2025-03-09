<template>
  <h1>[Vue.js Watch]</h1>
  <button @click="changeMessage">{{ message }}</button>
  {{ watchMessage }}
</template>
<script>
export default {
  name: 'Watch',
  data() {
    return {
      message: "안녕하세요, Vue.js Watch 기능 테스트 오리지널 문구",
      watchMessage: ''
    }
  },
  methods: {
    /* changeMessage() {
      console.log('함수 호출')
      this.message = '변경된 메시지'
    } */
    changeMessage: function() {
      console.log('함수 호출')
      this.message = '변경된 메시지'
    }
  },
  watch: {
    message(oldValue, newValue) { // 함수처럼 사용하지만 message라는 data 변수를 참조
        window.alert('message 변수에 담긴 데이터가 변경되었습니다.')
        this.watchMessage = 'Watch 동작'
    }
  }
}
</script>