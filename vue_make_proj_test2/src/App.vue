<template>
  <div id="app">
    <img src="./assets/logo.png">
    <div>{{testdata}}</div>
    <input type="text" v-bind:value="testFn" />
    <router-view/>
  </div>
</template>

<script>
export default {
  name: 'App',
  data: () => {
    return { testdata: 'aaaaaaaaa' }
  },
  computed: {
    testFn: () => {
      return '이거슨~~~'
    }
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
