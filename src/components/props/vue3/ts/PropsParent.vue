<template>
  <h1>[Vue.js Props]</h1>
  <Child 
    v-bind:sendProps1="title"
    v-bind:sendProps2="createAt"
    :sendProps3="obj"
  />
</template>
<script setup lang="ts">
import { reactive, ref } from 'vue';
import Child from './Child.vue'; // vue3를 지원하지 않는 vetur에서 export되지 않은 컴포넌트에 대한 이슈 무시가능
interface IObject {
  id: number;
  name: string;
}
const title = ref<string> ('부모 컴포넌트에서 선언된 데이터 입니다.');
const createAt = ref<number> (2025);
const obj = reactive<IObject> ({
  id: 2025,
  name: 'yooHyeok'
});
</script>