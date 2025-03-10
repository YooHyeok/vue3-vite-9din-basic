<template>
  <h1>[Vue.js Emits]</h1>
  <Child 
    @send-event="preventEvent"
  />
</template>
<script>
import Child from './Child.vue';
export default {
  name: 'EmitsParent',
  components: {
    Child
  },
  methods: {
    preventEvent(event) { // event에서 data를 받는다.
      console.log(event)
    }
  }
}
</script>