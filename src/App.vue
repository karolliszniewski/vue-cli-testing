<template>
<h1 type="text" ref="title">Hello</h1>
<button @click="handleClick">Click</button>
<Modal :header="header" :text="text" theme="sale"/>
</template>

<script>

import Modal from './components/AppModal.vue';

export default {
  name: 'App',
  components: {Modal},
data(){
  return{
    title:'My First Vue App',
    header:'Sign Up for the Giveaway',
    text: "some text",
   
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
