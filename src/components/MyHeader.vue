<template>
   <div> 
     <MyNavbar/>
     <MyJambo/>
   </div>
    
    
 
    
  
</template>

<script>


import MyNavbar from '@/components/MyNavbar.vue'; 
import MyJambo from '@/components/MyJambo.vue';  


export default {
    name:'MyHeader',
    
    components: {
        MyNavbar, 
        MyJambo      
  }

}
</script>

<style lang="scss">
  

</style>