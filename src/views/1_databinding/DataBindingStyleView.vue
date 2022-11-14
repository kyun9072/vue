<template>
  <div>
    <div :style="style1">스타일 바인딩: 글씨 빨간색, 폰트 30픽셀</div>
    <div :style="style2">스타일 바인딩: 글씨 녹색, 폰트 30픽셀</div>
    <button @click="style1.color = 'blue'">색상 변경</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      style1: { color: 'red', 'font-size': '30px' },
      style2: { color: 'green', 'font-size': '30px' }
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {}
}
</script>
