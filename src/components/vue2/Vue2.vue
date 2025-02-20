<template>
  <LifeCycle/>
  <VHtml/>
  <BindClass/>
</template>

<script>
import LifeCycle from './LifeCycle.vue';
import VHtml from './VHtml.vue';
import BindClass from './BindClass.vue';
export default {
  name: 'Vue2',
  components: {
    LifeCycle,
    VHtml,
    BindClass
  }
  
}
  
</script>

<style scoped></style>