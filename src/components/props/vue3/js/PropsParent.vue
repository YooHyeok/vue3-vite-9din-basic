<template>
  <h1>[Vue.js Props]</h1>
  <Child 
    v-bind:sendProps1="title"
    v-bind:sendProps2="createAt"
    :sendProps3="obj"
  />
</template>
<script setup lang="ts">
import Child from './Child.vue';
import { reactive, ref } from 'vue';
const title = ref ('부모 컴포넌트에서 선언된 데이터 입니다.');
const createAt = ref (2025);
const obj = reactive ({
  id: 2025,
  name: 'yooHyeok'
});
</script>