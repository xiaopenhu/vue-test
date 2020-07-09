<template>
  <div id="app">
    <div>
    <p :class="{ a: isA,b: isB}">使用 class</p>
    <p :class="[black,yellow]">使用 class (数组)</p>
    <p :style="styleDate"> 使用 style</p>
    <p v-bind:style="styleDate">使用</p>
  </div>
    <div>
      <p v-if="type === 'a'">A</p>
      <p v-else-if="type === 'b'">B</p>
      <p v-else-if="type === 'c'">C</p>
      <p v-else>other</p>
    </div>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      isA: true,
      isB: false,
      black: 'cblack',
      yellow: 'cyellow',
      styleDate: {
        fontSize: '40px',
        color: 'red',
        backgroundColor: '#ccc',
        type: 'a'
      }
    }
  }
}
</script>
<style>
</style>
