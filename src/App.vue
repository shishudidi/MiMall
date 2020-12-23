<template>
  <div id="app">
    <img alt="Vue logo" src="./assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import axios from "axios"
export default {
  name: 'app',
  components: {
    HelloWorld
  },
  mounted(){
    let url="https://www.fastmock.site/mock/871b3e736e653b99374b7713e4011f9f/boss/user/list";
    axios.get(url).then(()=>{})
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
