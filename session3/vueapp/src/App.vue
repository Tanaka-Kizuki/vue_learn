<template>
  <div id="app">
    <HelloWorld v-bind:title="message"/>
    <hr>
    <button v-on:click="doAction">Change Title</button>
  </div>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'

export default {
  name: 'App',
  components: {
    HelloWorld
  },
  data: function() {
    return {
      message:"HELLO",
    };
  },
  methods: {
    doAction:function() {
      var input = prompt("new title:");
      this.message = input;
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
