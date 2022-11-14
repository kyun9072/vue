<template>
  <div>
    <input type="text" name="" id="" :value="userId" readonly />
    <br />
    <img style="width: 100px; height: auto" :src="imgSrc" />
    <br />
    <input type="search" name="" id="" v-model="txtOne" />
    <button :disabled="check(txtOne)">조회</button>
  </div>
</template>
<script>
export default {
  components: {},
  data() {
    return {
      userId: 'avd',
      imgSrc: 'https://avatars.githubusercontent.com/u/6128107?s=280&v=4',
      txtOne: ''
    }
  },
  created() {},
  mounted() {},
  unmounted() {},
  methods: {
    check(str) {
      if (str.length > 3) {
        return false
      } else {
        return true
      }
    }
  }
}
</script>
