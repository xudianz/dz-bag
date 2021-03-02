<template>
  <div id="app">
    <DzBag :value="100" />
  </div>
</template>

<script>
import DzBag from '../src/bag/bag'
console.log(DzBag)

export default {
  name: 'app',
  components: {
    DzBag
  },
  data () {
    return {
      msg: 'Welcome to Your Vue.js App'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}
* {
  margin: 0;
  padding: 0;
  list-style: none;
}
</style>
