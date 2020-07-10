<template>
  <div id="app">
    <el-switch
      v-model="value"
      active-color="#13ce66"
      inactive-color="#ff4949">
    </el-switch>
    <HelloWorld>
      {{msg2}}
    </HelloWorld>
  </div>
</template>
<script>
import HelloWorld from './components/HelloWorld'
export default {
  data: function () {
    return {
      msg2: '我是父组件的值',
      value: true
    }
  },
  components: {
    HelloWorld
  }
}
</script>
