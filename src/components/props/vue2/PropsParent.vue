<template>
  <h1>[Vue.js Props]</h1>
  <child 
    v-bind:sendProps1="title"
    v-bind:sendProps2="createAt"
    :sendProps3="obj"
  />
</template>
<script>
import Child from './Child.vue';
export default {
  name: 'PropsParent',
  components: {
    Child
  },
  data() {
    return {
      title: "부모 컴포넌트에서 선언된 데이터 입니다.",
      createAt: 2025,
      obj: {
        id: 2025,
        name: 'yooHyeok'
      }
    }
  }
}
</script>