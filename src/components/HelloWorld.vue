<template>
  <div class="hello">
    <p>我是子组件hello world</p>
    <p>{{aa}}</p>
  </div>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: ['aa']
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
