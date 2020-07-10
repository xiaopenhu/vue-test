<template>
  <div class="hello" >
    <p>我是子组件hello world</p>
    <p>
      <slot></slot>
    </p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  data: function () {
    return {
      msg: '我是传给爸爸的儿子'
    }
  }
}
</script>
<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.hello{
  width: 200px;
  height: 200px;
  background: red;
}
</style>
