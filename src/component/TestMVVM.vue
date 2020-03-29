<template>
  <div>
    <h2>MVVM样例</h2>
    <p>{{msg}}</p>
    <label>
      <input type="text" v-model="msg" />
    </label>
  </div>
</template>
<script>
export default {
  data() {
    return {
      msg: "修改此处数据页面将同步改变"
    };
  }
};
</script>
<style></style>