<template>
  <button @click="sendEvent">자식 컴포넌트 버튼 - 콘솔출력</button>
</template>
<script>
export default {
  name: 'Child',
  data() {
    return {
      data: "자식 컴포넌트에서 선언된 데이터"
    }
  },
  methods: {
    sendEvent() {
      this.$emit('send-event', this.data)
    }
  }
}
</script>