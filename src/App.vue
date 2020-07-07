<template>
  <div id="app">
    <p>{{msg1}}</p>
    <p v-text="msg2"></p>
    <p v-html="msg3"></p>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      msg1: '我是插值表达式',
      msg2: '<span style="color:red">我是v-text<span>',
      msg3: '<span style="color:red">我是v-html<span>'
    }
  }
}
</script>
<style>

</style>
