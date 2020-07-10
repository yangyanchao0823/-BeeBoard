<template>
  <van-swipe class="Carouset my-swipe" :autoplay="3000" indicator-color="white">
    <van-swipe-item>1</van-swipe-item>
    <van-swipe-item>2</van-swipe-item>
    <van-swipe-item>3</van-swipe-item>
    <van-swipe-item>4</van-swipe-item>
  </van-swipe>
</template>

<script>
export default {
  name: 'Carouset',
  props: {
    msg: String
  }
}
</script>

<style scoped>
.my-swipe .van-swipe-item {
    height: 200px;
    color: #fff;
    font-size: 20px;
    line-height: 200px;
    text-align: center;
    background-color: #39a9ed;
  }
</style>
