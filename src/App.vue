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
  <PropsParent/>
</template>

<script>
import LifeCycle from './components/LifeCycle.vue';
import VHtml from './components/VHtml.vue';
import BindClass from './components/BindClass.vue';
import BindStyle from './components/BindStyle.vue';
import VIf from './components/VIf.vue';
import VShow from './components/VShow.vue';
import VForArr from './components/VForArr.vue';
import VForObj from './components/VForObj.vue';
import EventHandle from './components/EventHandle.vue';
import Computed from './components/Computed.vue';
import Watch from './components/Watch.vue';
import PropsParent from './components/props/vue2/PropsParent.vue';
export default {
  name: 'App',
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
    PropsParent
  }
  
}
  
</script>

<style scoped></style>