<template>
  <div id="app">
   
    <Api></Api>
  </div>
</template>

<script>
import Api from './components/Api.vue'

export default {
  name: 'App',
  components: {
    Api
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
body{
  background-color:darkslategrey;
}
h3{
  font-family: 'Courier New', Courier, monospace;
  font-size: 40px;
  color : rgb(92, 49, 18);
}
li.nameTag{
  font-family:'Courier New', Courier, monospace;
  font-size: 45px;
  color: teal;
}
li{
  font-family: 'Courier New', Courier, monospace;
  font-size: 20px;
  color:peru;
}
</style>
