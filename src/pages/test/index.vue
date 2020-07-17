<template>
  <view class="index">
    <NumberDisplay/>
    <NumberSubmit/>
  </view>
</template>

<script>
import NumberDisplay from '../../components/NumberDisplay.vue'
import NumberSubmit from '../../components/NumberSubmit.vue'

import mixin from '../../mixins/test.js'

export default {
  name: 'Index',
  components: {
    NumberDisplay,
    NumberSubmit
  },
  mixins: [mixin],
  created: function () {
    console.log(this)
    this.log('牛逼了')
    // => { message: "goodbye", foo: "abc", bar: "def" }
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
