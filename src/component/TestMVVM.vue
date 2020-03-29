<template>
  <div>
    <h1>{{msg}}</h1>
    <p></p>
    <label>
      <input type="text" v-model="msg" />
    </label>
  </div>
</template>
<script>
export default {
  data() {
    return {
      msg: "hhhhhhhhhh"
    };
  }
};
</script>
<style></style>