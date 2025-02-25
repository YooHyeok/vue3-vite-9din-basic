<template>

  <div>
    <div>Vue.JS v-for directive</div> 
    <li v-for="(item, idx) in objectArray" :key="idx">
      <span v-for="(value, key) in item" :key="key" > {{ key }} : {{ value }}</span>
    </li>
  </div>
</template>
<script>
export default {
  name: 'VForObj',
  data() {
    return {
      objectArray: [
        {id: 0, name: 'John'},
        {id: 1, name: 'Kim'},
        {id: 2, name: 'Lee'},
        {id: 3, name: 'Park'}
      ]
    }
  }
}
</script>