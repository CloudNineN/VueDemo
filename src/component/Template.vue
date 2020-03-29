<template>
  <div>
    <h2>双括号表达式 {{}}</h2>
    <p>
      {{"原始数据======"+intro}}
      <br />
      {{"原始数据+111======"+intro+111}}
      <br />
      {{"原始数据.touppercase======"+intro.toUpperCase()}}
      <br />
      {{"原始数据.tolowercase======"+intro.toLowerCase()}}
      <br />
    </p>
    <h2>强制数据绑定 v-model</h2>
    <p>
      <input type="text" v-model="site" />
      <br />
      <!-- <a v-bind:href="site">前往网站</a> -->
      <!-- 可用:简写v-bind -->
      <a :href="site">前往网站</a>
    </p>
    <h2>
      绑定事件监听 v-on
    </h2>
    <p>
      <input type="text" v-model="param" />
      <!-- <button v-on:click="Respond(param)" >button</button> -->
      <!-- 可用@简写v-on: -->
      <button @click="Respond(param)">button</button>
    </p>
  </div>
</template>

<script>
export default {
  name: "Template",
  data() {
    return {
      intro: "DATAdata",
      site: "https://www.baidu.com",
      param: ""
    };
  },
  methods: {
    Respond(s) {
      alert(s);
    }
  }
};
</script>

<style>
</style>