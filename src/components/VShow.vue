<template>
  <div>
    <h1>[Vue.JS v-show directive]</h1>
    <p>count {{ count }}</p>
    <div class="red" v-show="isVisable"></div> <!-- [비활성] style="display: none;" 적용. -->
    <div class="blue" v-show="!isVisable"></div> <!-- [활성] -->
    <div class="black" v-if="isVisable"></div> <!-- [비활성] 브라우저 요소에 v-if 라는 주석 생성 -->
  </div>
  <!-- v-show는 항상 렌더링되며 display css속성으로 전환됨. [초기렌더링비용↑] -->
  <!-- v-if는 truthy 값에서만 렌더링됨. - [전환비용↑] -->
  <!-- 매우 자주 전환될 경우 v-show / 실행중 조건이 변경되지 않는 경우 v-if -->
</template>
<script>
export default {
  name: 'VShow',
  data() {
    return {
      isVisable: false,
      count: 0,
    }
  }
}
</script>
<style scoped>
.red {
  width: 100px;
  height: 100px;
  background-color: red;
}
.blue {
  width: 100px;
  height: 100px;
  background-color: blue;
}
.black {
  width: 100px;
  height: 100px;
  background-color: black;
}
.pupple {
  width: 100px;
  height: 100px;
  background-color: blueviolet;
}
.yellow {
  width: 100px;
  height: 100px;
  background-color: yellow;
}
</style>