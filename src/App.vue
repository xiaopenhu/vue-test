<template>
  <div id="app">
    <HelloWorld @aa="fa">
      {{msg2}}
    </HelloWorld>
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
  }
}
</script>
