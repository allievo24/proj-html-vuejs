<template>
  <section class="quarta">
    <div class="containerCard">
      <div class="card" v-for="(person , index) in teams" :key="index" :teams="teams">
       <div class="img">
          <!-- 
            <img :src="require('@/assets/img/'+ person.img)+'.jpg'" alt="">
            <img  :src="require + (person.img)" alt=/>
            <img :src="require(`${person.img}`)" alt="">
            <img src="'@/assets/img/team-4.jpg'" alt="">
            <img :src="require(`${person.img}`)" alt="">
            <img src="'../assets/img/news-4.jpg'" alt="">
            <img :src="'@/assets/img/team-4.jpg'" alt="">
            <img :src="require(`@/assets/img/${person.img}`)" alt="">
            <img :src="'@/assets/img/team-4.jpg'" alt="">
          -->
          <img src="@/assets/img/team-1.jpg" alt="">
       </div>
       <div class="info">
          <h4>{{person.nome}}</h4>
          <h4>{{person.job}}</h4>
       </div>
      
      
    </div>
    </div>
    
  </section>
</template>

<script>
export default {
    name:'MyquartaSection',
    props:{
       teams:Array
    }

}
</script>

<style lang="scss">
.quarta{
  .containerCard{
    width: 70%;
    display: flex;
    flex-wrap: wrap;
    margin: auto;
    border: 2px solid yellow;

  }

//
border: 2px solid red;
.card{
  width: calc(100% / 2 - 1rem);
  border: 2px solid green;
  display: flex;
  margin: auto;



  .info{

  }



  
}

}

  img{
    width: 150px;
    height: 150px;
  }

</style>