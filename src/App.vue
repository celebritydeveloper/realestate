<template>
  <div id="app">
    <Index />
  </div>
</template>

<script>
//import HelloWorld from './components/HelloWorld.vue';
//import Register from './components/Register';
import Index from './components/Index';


export default {
  name: 'App',
  components: {
    //HelloWorld,
    //Register,
    Index,
  }
}
</script>

<style lang="scss">

$black: rgb(65, 76, 83);
$white: rgb(255,255,255);
/* width */
::-webkit-scrollbar {
  width: 5px;
}

/* Track */
::-webkit-scrollbar-track {
  background: #f1f1f1;
}

/* Handle */
::-webkit-scrollbar-thumb {
  background: rgb(65, 76, 83);
}

/* Handle on hover */
::-webkit-scrollbar-thumb:hover {
  background: rgb(65, 76, 83);
}

#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  color: #2c3e50;
  margin: 0;
  padding: 0;
}
</style>
