<template>
<h1 type="text" ref="title">Hello</h1>
<button @click="handleClick">Click</button>
</template>

<script>


export default {
  name: 'App',
data(){
  return{
    title:'My First Vue App'
  }
},
methods:{
  handleClick(){
    
    this.$refs.title.classList.add("hey")
    console.log(this.$refs.title)
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
