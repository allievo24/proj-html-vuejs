<template>
  <section class="terza">
    <div class="container">
     <span>OUR BUSINESS AREAS</span>
     <h3>Excellence in Services</h3>
     <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Deleniti aut odio temporibus sed nostrum libero quisquam doloribus ad laudantium nulla quaerat ab quidem porro tempora culpa adipisci, fuga error quis?</p>
      <div class="containerCard">
          <div class="card" v-for="(card , index) in cards" :key="index" :cards="cards">
          <span><i :class= card.icone></i></span>
          <span><i class="fa-solid fa-arrow-right"></i></span>
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
 
  .containerCard{
    display: flex;
    flex-wrap: wrap;
    .card{
      width: calc(100% / 3 - 5rem);
      height:200px;
      padding: 3rem;
      margin: auto;
      margin-bottom:2rem;
      margin-top:2rem;
      border: 2px solid ;
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