<template>
  <view class="content">
    <view>
      我是test组件

      <view>
        我是来自 index.vue组件的变量
        {{ TEST }}
      </view>
    </view>
  </view>
</template>

<script>
import { TEST } from "./index"
export default {
  data() {
    return {
      TEST,
      title: "Hello",
    }
  },
  onLoad() {},
  methods: {},
}
</script>

<style>
.content {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
}

.logo {
  height: 200rpx;
  width: 200rpx;
  margin: 200rpx auto 50rpx auto;
}

.text-area {
  display: flex;
  justify-content: center;
}

.title {
  font-size: 36rpx;
  color: #8f8f94;
}
</style>
