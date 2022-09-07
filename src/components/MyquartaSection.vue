<template>
  <section class="quarta">
    <div class="card" v-for="( person , index) in teams" :key="index" :teams="teams">
      <!--<img :src="'../assets/img/'+ person.img " alt="">
       <img src="src/assets/img/team-1.jpg" alt="">-->
       <img src="src/assets/img/bg-1.jpg" alt="">

      <h4>{{person.job}}</h4>
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

<style>

</style>