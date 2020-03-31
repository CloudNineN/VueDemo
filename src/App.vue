<template>
  <div class="demo">
    <h1>组件1</h1>
    <TestMVVM />
    <p>=====================================================</p>
    <h1>组件2</h1>
    <Template />
    <p>=====================================================</p>
    <h1>组件3</h1>
    <ComputedAndWatch />
    <p>=====================================================</p>
    <h1>组件4</h1>
    <ClassAndStyle />
  </div>
</template>

<script>
import Template from "./component/Template";
import TestMVVM from "./component/TestMVVM";
import ComputedAndWatch from "./component/ComputedAndWatch";
import ClassAndStyle from "./component/ClassAndStyle";
export default {
  name: "app",
  components: {
    Template,
    TestMVVM,
    ComputedAndWatch,
    ClassAndStyle
  }
};
</script>

<style>
</style>
