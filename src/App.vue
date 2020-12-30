<template>
<div id="app">
  Welcome {{user.username}} - The current time is - {{currentTime}}
</div>
</template>

<script>


export default {
  name: 'App',
  data(){
    return{
      followers: 0,
      user: {
        id: 1,
        username: 'djp'
      }
    }
  },
  computed:{
    currentTime(){
      return Date();
    }
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
