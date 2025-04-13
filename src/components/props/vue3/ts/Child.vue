<template>
  <div>{{ props.sendProps1 }}</div>
  <div>{{ props.sendProps2 }}</div>
  <div>{{ props.sendProps3.id }}</div>
  <div>{{ props.sendProps3.name }}</div>
  <!-- Props 정규화 -->
  <div>{{ sendProps1 }}</div>
  <div>{{ sendProps2 }}</div>
  <div>{{ sendProps3.id }}</div>
  <div>{{ sendProps3.name }}</div>
</template>
<script setup lang="ts">

interface IObject {
  id: number;
  name: string;
}
interface IProps {
  sendProps1: String,
  sendProps2: Number,
  sendProps3: IObject,
}
/* 
defineProps의 경우 vue3에서는 내장되어있기 때문에 import 하지 않아도 된다.
정확히는 Vite에서 vue3를 사용할 때 생략이 가능하다.  
여전히 Webpack을 사용하는 Vue CLI를 통해 Vue3 프로젝트를 생성할 경우 생력할 수 없다.  

 */
const props = defineProps<IProps>()
</script>