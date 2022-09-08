<template>
<section class="quinta">
    <div class="container">
        <div class="left"></div>
        <div class="right"></div>
    </div>
    <div class="containerCard">
        <div class="card" v-for="(New , index) in News" :key="index" :News="News">
           <img :src="New.img" alt="">
           {{New.p}}
        </div>
    </div>
</section>
  
</template>

<script>
export default {
     name:'MyquintaSection',
     props:{
      News:Array
     }   

}
</script>

<style lang="scss">
.quinta{
    background-color:rgb(238, 244, 237) ;
   // height: 700px;
  .container{
    border:2px solid red;
    height: 100%;
    width: 90%;
    margin: auto;
    .left{
        border:2px solid blue;
        height: 20px;
       
    }
    .right{
       border:2px solid blue;
       height: 20px; 
    }
  }
  .containerCard{
    width: 90%;
    margin: auto;



    .card{
       border:2px solid rgb(0, 255, 72);
       height: 100px;

    }
  }
}

</style>