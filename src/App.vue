<template>
  <div id="app">
    <ChinaSeventy/>
  </div>
</template>

<script>
import ChinaSeventy from './components/ChinaSeventy.vue'
export default {
  name: 'app',
  components: {
    ChinaSeventy,
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  text-align: center;
  background-color: #eee;
  height: 100%;
}
</style>
