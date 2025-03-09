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
  <Computed/>
  <Watch/>
  <Parent/>
</template>

<script>
import LifeCycle from './LifeCycle.vue';
import VHtml from '../vue2/VHtml.vue';
import BindClass from '../vue2/BindClass.vue';
import BindStyle from '../vue2/BindStyle.vue';
import VIf from '../vue2/VIf.vue';
import VShow from '../vue2/VShow.vue';
import VForArr from '../vue2/VForArr.vue';
import VForObj from '../vue2/VForObj.vue';
import EventHandle from '../vue2/EventHandle.vue';
import Computed from '../vue2/Computed.vue';
import Watch from '../vue2/Watch.vue';
// import Parent from './props/Parent.vue';
import Parent from './vue2/emits/EmitsParent.vue';
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
    Computed,
    Watch,
    Parent
  }
  
}
  
</script>

<style scoped></style>