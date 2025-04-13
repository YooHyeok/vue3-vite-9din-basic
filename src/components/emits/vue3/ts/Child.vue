<template>
  <button @click="sendEvent">자식 컴포넌트 버튼 - 콘솔출력</button>
</template>
<script setup lang="ts">
import { ref } from 'vue'

const data = ref<string>('자식 컴포넌트에서 선언된 데이터')
const emits = defineEmits(['send-event']) // vue3 Emit 등록
const sendEvent = () => {
      emits('send-event', data.value) // this.$emit('send-event', this.data)
    }
</script>