<template>
  <div>
    <div
      :class="{ 'text-red': hasError, active: isActive }"
      v-on:mouseover="hoverMouse"
      v-on:mouseleave="leaveMouse"
    >
      이벤트제어 때문에 실무에선 내가 더 많이 쓰임
    </div>
    <div
      :class="{ 'text-green': hasOn, active1: hasLeave }"
      @mouseover="hasOnFc"
      @mouseleave="hasLeaveFc"
    >
      이벤트제어 때문에 실무에선 내가 더 많이 쓰임2
    </div>
    <div :class="css">클래스 바인딩</div>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      isActive: false,
      hasError: false,
      hasOn: false,
      hasLeave: false,
      css: ['active', 'text-red']
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    hoverMouse() {
      this.isActive = true
      this.hasError = true
    },
    leaveMouse() {
      this.isActive = false
      this.hasError = false
    },
    hasOnFc() {
      this.hasOn = true
      this.hasLeave = true
    },
    hasLeaveFc() {
      this.hasOn = false
      this.hasLeave = false
    }
  }
}
</script>
<style scoped>
.active {
  background-color: greenyellow;
  font-weight: bold;
}
.text-red {
  color: red;
}
.active1 {
  background-color: green;
  font-weight: bold;
}
.text-green {
  color: green;
}
</style>
