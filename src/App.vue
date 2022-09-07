<template>
  <div id="app">
   <MyHeader/>,
   <MyMain :links="links"/>
   <MyFooter/>
   
  </div>
</template>

<script>
import MyMain from '@/components/MyMain.vue';
import MyFooter from '@/components/MyFooter.vue';
import MyHeader from '@/components/MyHeader.vue'







export default {
  name: 'App',
  components: {
   MyHeader,
   MyMain,
   MyFooter
  },
    data(){
        return{
           links:[
             
             {
               text:'Certification',
               number:'120', 
               url:'#'

             },
              {
               text:'Employees',
               number:'230', 
               url:'#'

             },
              {
               text:'Custromers',
               number:'517', 
               url:'#'

             },
             {
               text:'Countries Served',
               number:'94', 
               url:'#'

             },
           ] 
        }
    },
}


</script>

<style lang="scss">
    @import '~@fortawesome/fontawesome-free/css/all.css';
    @import './styles/generali.scss';
     
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
 
}
</style>
