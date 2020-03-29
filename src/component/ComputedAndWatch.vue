<template>
  <div>
    <h2>计算属性 computed</h2>
    <p>
      <input type="text" v-model="site" />
      <br />当前地址
      <a :href="fullSite">{{fullSite}}</a>
    </p>
    <h2>监听属性 watch</h2>
    <p>
      <input type="text" v-model="site2" />
      <br />当前地址
      <a :href="fullSite2">{{fullSite2}}</a>
    </p>
    <h2>反转字符串 .split("").reverse().join("")</h2>
    <p>
      <input type="text" v-model="reverse" />
      <br />
      {{reversed}}
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
      after: ".com",
      site2: "",
      fullSite2: "",
      reverse: "",
      reversed: ""
    };
  },
  computed: {
    fullSite: {
      get() {
        return this.before + this.site + this.after;
      }
    }
  },
  watch: {
    site2(v) {
      if (v == "天王盖地虎") {
        alert("宝塔镇河妖");
      }
      this.fullSite2 = this.before + v + this.after;
    },
    reverse(v) {
      this.reversed = v
        .split("")
        .reverse()
        .join("");
      if (v.length > 1 && v == this.reversed) {
        this.reversed += " 回文！";
      }
    }
  }
};
</script>
<style></style>