<template>
  <div class="demo">
    <h1>组件1</h1>
    <TestMVVM />
    <p>=====================================================</p>
    <h1>组件2</h1>
    <Template />
    <p>=====================================================</p>
    <h1>组件3</h1>
    <ComputedAndWatch/>
    <p>=====================================================</p>
  </div>
</template>

<script>
import Template from "./component/Template";
import TestMVVM from "./component/TestMVVM";
import ComputedAndWatch from "./component/ComputedAndWatch";
export default {
  name: "app",
  components: {
    Template,
    TestMVVM,
    ComputedAndWatch
  }
};
</script>

<style>
</style>
