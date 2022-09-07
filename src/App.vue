<template>
  <div id="app">
   <MyHeader/>,
   <MyMain :links="links" :cards="cards" />
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
           ],
           cards:[
                  { icone:"fa-solid fa-network-wired",
                    titolo:'Audit & Assurance',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                  },
                  {
                    icone:"fa-solid fa-briefcase",
                    titolo:'Financial Advisory',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                  },
                  
                  { 
                    icone:"fa-solid fa-chart-simple",
                    titolo:'Analytics and M&A',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                  },
                  {
                    icone:"fa-solid fa-plane",
                    titolo:'Middele Marketing',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                  },
                  {
                    icone:"fa-solid fa-globe",
                    titolo:'Legal Consulting',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                  },
                  {
                    icone:"fa-solid fa-hard-drive",
                    titolo:'Regulatory Risk',
                    text:'Lorem ipsum dolor sit amet consectetur adipisicing elit.'
                  }
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
