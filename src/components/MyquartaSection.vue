<template>
  <section class="quarta">
    <div class="card" v-for="(person , index) in teams" :key="index" :teams="teams">
       <div class="img">
       <img  :src="require(`@/assets/img/${person.img}.jpg`)" alt=/>
       <img :src="require(person.img)+'.jpg'" alt="">
       
       </div>
      <h4>{{person.nome}}</h4>
      <h4>{{person.job}}</h4>
      
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
  img{
    width: 100px;
    height: 100px;
  }

</style>