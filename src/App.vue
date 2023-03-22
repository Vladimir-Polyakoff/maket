<script>
import Header from '@/views/Header'

export default {
  name: 'TheApp',

  components: {
    Header
  }
}
</script>

<template>
  <div id="app">
    <Header></Header>
    <!-- <router-view/> -->
  </div>
</template>

<style lang="scss">
body {
  margin: 0;
  padding: 0;
  background: #E5E5E5;

}
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  max-width: 1440px;
  height: 100%;
  margin: 0 auto;
  background: #fff;
}
</style>
