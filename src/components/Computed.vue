<template>
  <h1>[Computed]</h1>
  <div>
    <h2>{{ text }}</h2>
    <h2>changeText() 호출 값: {{ changeText() }}</h2>
    <h2>changeText() 호출 값: {{ changeText() }}</h2>
    <h2>changeText() 호출 값: {{ changeText() }}</h2>
    <h2>computedText 호출 값: {{ computedText }}</h2>
    <h2>computedText 호출 값: {{ computedText }}</h2>
    <h2>computedText 호출 값: {{ computedText }}</h2>
  </div>

</template>
<script>
/* 

*/
export default {
  name: 'Computed',
  data() {
    return {
      text: "Computed 테스트 데이터 문구입니다."
    }
  },
  methods: {
    changeText() {
      console.log("함수 호출") // 3번 호출
      console.log(this.text)
      return this.text.split("").reverse().join("") // 빈칸을 기준으로 분할 - 역순정렬 - 문자열재조합
    }
  },
  computed: { 
    computedText() {
      console.log("Computed 기능을 생성 하였습니다. 호출") // 1번 호출
      console.log(this.text)
      return this.text.split("").reverse().join("") // 빈칸을 기준으로 분할 - 역순정렬 - 문자열재조합
    }
  }
}
</script>