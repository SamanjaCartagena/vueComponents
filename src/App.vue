<template>
 <GreetT />
</template>

<script>
import GreetT from './components/GreetT.vue';
export default {
  name: 'App',
  components: {
    GreetT
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
