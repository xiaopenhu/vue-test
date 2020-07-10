<template>git
  <div id="app">
    <p>{{msg2}}</p>
    <HelloWorld @aa="fa"></HelloWorld>
  </div>
</template>
<script>
import HelloWorld from './components/HelloWorld'
export default {
  data: function () {
    return {
      msg2: '我是父组件的值'
    }
  },
  components: {
    HelloWorld
  },
  methods: {
    fa: function (val) {
      this.msg2 = val
    }
  }
}
</script>
