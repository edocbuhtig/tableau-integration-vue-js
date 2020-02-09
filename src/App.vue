<template>
  <div id="app">
    
    <TableauHolder msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import TableauHolder from './components/TableauHolder'

export default {
  name: 'App',
  components: {
    TableauHolder
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
