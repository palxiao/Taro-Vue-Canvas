<template>
  <view class="index">
    <my-swiper @tap="openEditor" @change="swiperChange" :imgUrls="imgUrls" />
  </view>
</template>

<script>
import MySwiper from '../../components/bussiness/SelectModel.vue'

export default {
  name: 'Index',
  components: {
    MySwiper
  },
  mixins: [],
  created () {
    
  }
}
</script>

<style>
.index {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
