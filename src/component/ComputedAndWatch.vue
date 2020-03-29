<template>
  <div>
    <h2>
      计算属性 computed
    </h2>
    <p>
      <input type="text" v-model="site" />
      <br />当前地址
      <a :href="fullSite">{{fullSite}}</a>
    </p>
  </div>
</template>
<script>
export default {
  name: "ComputedAndWatch",
  data() {
    return {
      site: "baidu",
      before: "https://",
      after: ".com"
    };
  },
  computed: {
    fullSite: {
      get() {
        return this.before + this.site + this.after;
      }
    }
  }
};
</script>
<style></style>