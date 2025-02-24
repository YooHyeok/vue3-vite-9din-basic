<template>
  <LifeCycle/>
  <VHtml/>
  <BindClass/>
  <BindStyle/>
  <VIf/>
  <VShow/>
</template>

<script>
import LifeCycle from './LifeCycle.vue';
import VHtml from './VHtml.vue';
import BindClass from './BindClass.vue';
import BindStyle from './BindStyle.vue';
import VIf from './VIf.vue';
import VShow from './VShow.vue';
export default {
  name: 'Vue2',
  components: {
    LifeCycle,
    VHtml,
    BindClass,
    BindStyle,
    VIf,
    VShow
  }
  
}
  
</script>

<style scoped></style>