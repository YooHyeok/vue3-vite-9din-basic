<template>
  <div>{{ sendProps1 }}</div>
  <div>{{ sendProps2 }}</div>
  <div>{{ sendProps3.id }}</div>
  <div>{{ sendProps3.name }}</div>
</template>
<script>
export default {
  props: {
    sendProps1: String,
    sendProps2: Number,
    sendProps3: Object,
  },
  name: 'Child',
  data() {
    return {}
  }
}
</script>