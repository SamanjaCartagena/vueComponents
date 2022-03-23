<template>
<div>
 <GreetT />
 <ListS :listdata="items" @clickedItem="getClickedItem" />
 {{clickedItem}}
 </div>
</template>

<script>
import GreetT from './components/GreetT.vue';
import ListS from './components/ListS.vue';
export default {
  data: () => {
    return {
      items:['first', 'second', 'third'],
      clickedItem:''
    }
  },
  name: 'App', 
  
  components: {
    GreetT,
    ListS
  },
  methods:{
    getClickedItem(value){
         this.clickedItem = value;
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
