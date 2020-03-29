<template>
  <div class="demo">
    <TestMVVM/>
    <P></P>
    <Template/>
  </div>
</template>

<script>
import Template from './component/Template'
import TestMVVM from './component/TestMVVM'
export default {
  name: "app",
  components:{
    Template,
    TestMVVM
  }
};
</script>

<style>
</style>
