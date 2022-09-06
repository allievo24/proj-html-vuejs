<template>
  <div id="app">
   <MyHeader/>
  
   <MyMain/>
    <MyFooter/>
   
  </div>
</template>

<script>
import MyMain from '@/components/MyMain.vue';
import MyFooter from '@/components/MyFooter.vue';
import MyHeader from '@/components/MyHeader.vue';







export default {
  name: 'App',
  components: {
   MyHeader,
   MyMain,
   MyFooter
  }
}
</script>

<style lang="scss">
    @import "./styles/generali.scss";
    @import '~@fortawesome/fontawesome-free/css/all.css';
     
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
 
}
</style>
