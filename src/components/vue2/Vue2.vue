<template>
  <LifeCycle/>
  <VHtml/>
  <BindClass/>
  <BindStyle/>
  <VIf/>
  <VShow/>
  <VForArr/>
  <VForObj/>
  <EventHandle/>
</template>

<script>
import LifeCycle from './LifeCycle.vue';
import VHtml from './VHtml.vue';
import BindClass from './BindClass.vue';
import BindStyle from './BindStyle.vue';
import VIf from './VIf.vue';
import VShow from './VShow.vue';
import VForArr from './VForArr.vue';
import VForObj from './VForObj.vue';
import EventHandle from './EventHandle.vue';
export default {
  name: 'Vue2',
  components: {
    LifeCycle,
    VHtml,
    BindClass,
    BindStyle,
    VIf,
    VShow,
    VForArr,
    VForObj,
    EventHandle,
  }
  
}
  
</script>

<style scoped></style>