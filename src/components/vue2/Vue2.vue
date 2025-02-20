<template>
  <LifeCycle/>
  <VHtml/>
  <BindClass/>
  <BindStyle/>
</template>

<script>
import LifeCycle from './LifeCycle.vue';
import VHtml from './VHtml.vue';
import BindClass from './BindClass.vue';
import BindStyle from './BindStyle.vue';
export default {
  name: 'Vue2',
  components: {
    LifeCycle,
    VHtml,
    BindClass,
    BindStyle
  }
  
}
  
</script>

<style scoped></style>