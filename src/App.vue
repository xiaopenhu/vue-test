<template>
  <div id="app">
    <HelloWorld :aa="msg"></HelloWorld>
  </div>
</template>
<script>
import HelloWorld from './components/HelloWorld'
export default {
  data: function () {
    return {
      msg: '父组件传递给了我，所以我是子组件'
    }
  },
  components: {
    HelloWorld
  }
}
</script>
