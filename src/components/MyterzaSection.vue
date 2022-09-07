<template>
  <section class="terza">
    <div class="container">
     <span>OUR BUSINESS AREAS</span>
     <h3>Excellence in Services</h3>
     <div class="containerTitoli">
         <div class="testo">
          <p>We are leaders in providing consultancy services with a set of cutting-edge technologies and a team of //experienced and renowned professionals. These are some options that you can hire.</p>
         </div>
        <div class="botton">
          SELL ALL
        </div>   
     </div>
     
      </div>
      <div class="containerCard">
          <div class="card" v-for="(card , index) in cards" :key="index" :cards="cards">
          <span><i :class= card.icone></i></span>
          <span><i class="fa-solid fa-arrow-right"></i></span>
          <div class="desriptionCard">
            <h4>{{card.titolo}}</h4>
            <p>{{card.text}}</p>
          </div>
          
        </div>

      </div>
    
     

    

  </section>
</template>

<script>
export default {
    name:'MyterzaSection',
    props:{
      cards:Array
    }

}
</script>


<style lang="scss">
  @import '~@fortawesome/fontawesome-free/css/all.css';

.terza{
  border:2px solid red;
  background-color: rgb(17, 17, 23);
   .container{
     padding:2rem 3rem ;
     border: 2px solid red;
     .containerTitoli{
      display: flex;
      justify-content:space-between;
      align-items: center;
      color: white;
      .testo{
        width: 75%;
        border: 2px solid red;
      }
      .botton{
        border: 2px solid rgb(0, 171, 167);
        padding:0.5rem;
      }

   
     }
     span{
      color:rgb(0, 171, 167) ;
     }
     h3{
       color:white;
       }
     P{
      color: rgb(189, 190, 180);
      
       
     
      
      
     }
   }

 
  .containerCard{
    display: flex;
    flex-wrap: wrap;
    .desriptionCard{
          padding: 1rem 2rem 0 0;
          color:rgb(253, 252, 250);
          p{
            margin-top: 1rem;
            color: rgb(189, 190, 180)
          }

        }
    .card{
      width: calc(100% / 3 - 5rem);
      height:200px;
      padding: 3rem;
      margin: auto;
      margin-bottom:2rem;
      margin-top:2rem;
      border: 2px solid ;
      background-color: rgb(25, 25, 31);
      span{
        font-size: 1.5rem;
        color:rgb(3, 135, 134);
        .fa-arrow-right{
          margin-left:11rem ;
        }
        
      }
    }
  }
  

}
 

</style>