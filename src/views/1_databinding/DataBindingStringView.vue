<template>
  <div class="text-red">
    <h1>Hello, {{ userName }}</h1>
    <p>I {{ city }} U</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      userName: 'John Joe',
      age: 80,
      city: 'Seoul'
    }
  }
}
</script>
<style scoped>
.text-red {
  color: red;
}
</style>
