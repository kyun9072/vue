<template>
  <div class="home">
    <HelloWorld class="world1" msg="Welcome to Your Vue.js App" />
    <HelloWorld2 class="world2" msg="Welcome2" />
  </div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import HelloWorld2 from '@/components/HelloWordl2.vue'
export default {
  name: 'HomeView',
  components: {
    HelloWorld, HelloWorld2
  }
}
</script>
<style>
.world1 {
  float: left;
}

.world2 {
  float: right;
}
</style>
