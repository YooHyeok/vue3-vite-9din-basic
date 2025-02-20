<template>
  <div>{{ rawHtml }}</div>
  <div>{{ rawHtml2 }}</div>
  <h1 v-html="rawHtml2"></h1>
</template>
<script>
export default {
  name: 'VHtml',
  data() {
    return {
      rawHtml: '이것은 텍스트 입니다.',
      rawHtml2: '<span style="color: red;">이것은 빨간색 텍스트 입니다.</span>'
    }
  }
}
</script>