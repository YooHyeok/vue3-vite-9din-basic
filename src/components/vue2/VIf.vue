<template>
  <div>Vue.JS v-if directive
    <p>count {{ count }}</p>
    <div class="red" v-if="isVisable"></div>
    <div class="blue" v-if="isVisable == true"></div>
    <div class="black" v-else></div>

    <!-- v-if에 담긴 조건이 true일 때 활성화 되는것이지, 변수가 true일 때 활성화가 되는것은 아니다. -->

    <div class="pupple" v-if="count > 1"></div> <!-- 1보다 크면 보라색, 1보다 작거나 같으면 노란색 -->
    <div class="yellow" v-else></div>
    <button @click="count++">증가</button>
    <button @click="count--">감소</button>
  </div>
</template>
<script>
export default {
  data() {
    return {
      isVisable: true,
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