<template>

  <div>
    <div>Vue.JS v-for directive</div>  
    <!-- <li>{{ sampleArray[0] }}</li>
    <li>{{ sampleArray[1] }}</li>
    <li>{{ sampleArray[2] }}</li>
    <li>{{ sampleArray[3] }}</li> -->
    <li v-for="(item, idx) in sampleArray" :key="idx">{{ item }}</li>
  </div>
</template>
<script>
export default {
  name: 'VForArr',
  data() {
    return {
      sampleArray: ['a', 'b', 'c', 'd']
    }
  }
}
</script>