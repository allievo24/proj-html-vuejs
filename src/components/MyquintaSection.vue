<template>
<section class="quinta">
    <div class="container">
        <div class="left">
          <span>OUR EDITORIAL CONTENT'</span>
          <h2>Latest News</h2> 
                 
          <p> Everry week we publish content about what is best in the business world.'</p> 
        </div>
        <div class="right"></div>
    </div>
    <div class="containerCard">
        <div class="card" v-for="(New , index) in News" :key="index" :News="News">
          <!--<img :src="require(`@/assets/img/${New.img}.jpg`)" alt=""/>-->
          <img src="@/assets/img/news-1.jpg" alt=""> 
           <div class="text">
           <strong>{{New.text}}</strong> 
           </div>
          
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
       // height: 20px;
       
    }
    .right{
       border:2px solid blue;
       height: 20px; 
    }
  }
  .containerCard{
    width: 90%;
    margin: auto;
    display: flex;
    border: 3px solid ;
    margin-top:2rem ;
    



    .card{
       border:2px solid rgb(0, 255, 72);
     //  width: calc(100% / 3 - 2rem);
       margin: auto;
      // position:relative;
       img{
        width: 100%;
       // height: 100%;
       }
       .text{
       
          width: 66%;
          margin: auto;
          color: white;
          position: relative;
          bottom: 7rem;
          border: 2px solid;
          text-align: center;
          font-size: 21px;

          
    
       }

    }
  }
}

</style>