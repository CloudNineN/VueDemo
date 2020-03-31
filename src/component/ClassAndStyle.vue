<template>
  <div>
    <h2>动态样式绑定 Class</h2>
    <div :class="classOne">演示样例 演示样例 演示样例 演示样例 演示样例 演示样例 演示样例</div>
    <div :class="{classOneSytle:true,classTwoSytle:true}">演示样例 演示样例 演示样例 演示样例 演示样例 演示样例 演示样例</div>
    <div :class="{classTwoSytle:true}">演示样例 演示样例 演示样例 演示样例 演示样例 演示样例 演示样例</div>
    <div :class="[classOne,classTwo]">演示样例 演示样例 演示样例 演示样例 演示样例 演示样例 演示样例</div>
    <h2>动态样式绑定 Style</h2>
    <div
      :style="{'backgroundColor':bgColor,'fontSize': fSize,'font-weight':'bold'}"
    >演示样例 演示样例 演示样例 演示样例 演示样例 演示样例 演示样例</div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      classOne: "classOneSytle",
      classTwo: "classTwoSytle",
      bgColor: "skyBlue",
      fSize: "20px"
    };
  }
};
</script>

<style>
.classOneSytle {
  font-size: 20px;
  font-weight: bold;
  color: royalblue;
}
.classTwoSytle {
  width: 400px;
  height: 200px;
  background-color: skyblue;
  margin: 10px auto;
}
</style>