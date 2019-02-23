<template>
  <div id="app">
    <h1>Reactivity</h1>
    <p>{{ seconds }} have elapsed since this page is open.</p>
  </div>
</template>

<script>
export default {
  name: 'app',
  data () {
    return {
      seconds: 0
    }
  },
  // create runs when the app is initiated
  created () {
    setInterval( () => {
      this.seconds++;
    }, 1000);
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
