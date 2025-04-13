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
<script setup>
import { toRefs } from 'vue';

const props = defineProps({
  sendProps1: String,
  sendProps2: Number,
  sendProps3: {
    id: Number,
    name: String
  }
}) 
const {sendProps1, sendProps2, sendProps3} = toRefs(props) // props 정규화 (구조 분해 할당을 통해 간편하게 사용하도록 지원)
</script>