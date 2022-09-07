<template>
    <section class="seconda" >
        <div class="container" v-for="(link ,index) in links" :key="index" :links="links">
            <div class="titolo">
            <span>{{link.t1}}</span>
            <h2>{{link.t2}}</h2>
            </div>
            <div class="link">
                <ul>
                    <li>{{link.number}}</li> 
                    <li><a :href="link.url">{{link.text}}</a></li>
        
                </ul>
           </div>
        
        </div>

    </section>
</template>

<script>
export default {
    name :'MysecondSection',
    props:{
        links:Array
    }
  
}
</script>

<style lang="scss">
  
    section{
         
          border:2px solid red;
         
        
    }
    
    .container{
   
        border: 2px solid black;
       
      ul{
        text-align: center;
      }
      li{
        display:block;
        width: calc(100% / 4);
      border: 2px solid yellow;


        

      }
     
    }
  
  
   

</style>