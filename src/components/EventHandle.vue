<template>
  <h1>[Vue.js 이벤트 핸들링]</h1>
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
/* 
인라인 핸들러는 어떤 로직이 template즉, html 태그 안에 로직이 담겨있는것을 의미한다.  
함수 이름, 혹은 함수를 가리키는 경로가 아닌 간단한 로직 자체가 들어간다.
어떤 로직을 처리하는 부분이 script영역이 아닌 template html에 직접 바인딩되는 방식이다.

메소드 핸들러는 인라인 핸들러와 달리 로직 자체가 template html에 직접 바인딩되지 않고,  
methods영역에 따로 선언한 뒤 선언된 함수를 바인딩하여 관리하는 방식이다.  

데이터가 변경되는것이 중요한게 아니라 원하는 로직을 템플릿에서 처리하느냐, 스크립트에서 처리하느냐에 초점을 둔다.  
간단한 로직일 경우에는 인랑니 핸들러를 사용해도 무방하지만 조금 복잡한 로직일 경우에는 함수로 따로 분리하여 관리한다.  
*/
export default {
  name: 'EventHandle',
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