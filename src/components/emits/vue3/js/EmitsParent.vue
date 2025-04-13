<template>
  <h1>[Vue.js Emits]</h1>
  <Child 
    @send-event="preventEvent"
  />
</template>
<script setup>
import Child from './Child.vue';
const preventEvent = (event) => { // event에서 data를 받는다.
  console.log(event)
}
</script>