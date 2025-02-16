<template>
  <div>{{ count }}</div>
  <h1>Vue.js 라이프사이클 테스트</h1>
</template>

<script>
export default {
  name: 'App',

  data() {
    return {
      count: 0
    };
  },

  /* === 데이터와 관련 === */

  /**
   * 컴포넌트가 생성되기 전에 동작하는 라이프사이클 훅
   * data, methods에 선언한 데이터, 함수에 접근할 수 없다.
   */
  beforeCreate() {
    console.log("LifeCycle is beforeCrete", this.count) //  컴포넌트가 생성되기 전 이므로 undefined 출력
  },
  /**
   * 컴포넌트가 생성된 직후 접근할 수 있는 라이프사이클 훅
   * data, methods에 선언한 데이터, 함수에 접근 가능하다.
   */
  created() {
    console.log("LifeCycle is creted", this.count) // 컴포넌트가 생성된 후 초기화 진행되므로 0 출력
  },


  /* === Dom과 관련 === */
  
  /**
   * 컴파일된 template 유무와 관계 없이 초기 렌더링을 거치기 전에 동작하는 라이프사이클 훅
   * DOM이 렌더링 되기 전 이므로 template 영역의 HTML Element에 접근 불가능하다.
   */
  beforeMount() {
    console.log("LifeCycle is beforeMount", document.querySelector('h1')) // 렌더링 전 이므로 null 출력
  },
  /**
   * 컴포넌트, 템플릿, 렌더링된 DOM에 접근할 수 있고 DOM을 수정하기 위해 사용된다.
   * template 영역의 HTML Element가 모두 렌더링 된 후 접근이 가능하다.
   */
  mounted() {
    console.log("LifeCycle is mounted", document.querySelector('h1')) // 렌더링 직후 이므로 h1 태그 출력
  }
};
</script>

<style scoped></style>