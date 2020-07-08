<template>
  <div id="app">
    <div class="guding">
      <div style="width: 34%"></div>
      <div style="width: 11%" @click="change('/image/index.jpg')"></div>
      <div style="width: 18%" @click="change('/image/sxy.jpg')"></div>
      <div style="width: 15%"  @click="change('/image/hezuo.jpg')"></div>
      <div style="width: 21%" @click="change('/image/lianxi.jpg')"></div>
    </div>
    <div class="header">
      <img src="/image/header.jpg" alt="" width="100%">
    </div>
    <div class="index">
      <img :src="imgName" alt="" width="100%">
    </div>
    <div class="footer">
      <img src="/image/footer.jpg" alt="" width="100%">
    </div>
  </div>
</template>
<script>
export default {
  data: function () {
    return {
      imgName: '/image/index.jpg'
    }
  },
  methods: {
    change: function (name) {
      this.imgName = name
    }
  }
}
document.addEventListener('DOMContentLoaded', () => {
  const html = document.querySelector('html')
  const fontSize = window.innerWidth / 10
  html.style.fontSize = fontSize + 'px'
})
</script>
<style>
  .guding{
    height: 1rem;
    width: 100%;
    position: absolute;
    display: flex;
  }
  .guding div{
    height: 100%;
  }
  .header{
    height: auto;
    wight:100%;
  }
  .footer{
    height: auto;
    width: 100%;
  }
  .index{
    height: auto;
    width: 100%;
  }
</style>
