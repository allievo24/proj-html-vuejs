<template>
  <div>
    <MyprimSection/>
    <MysecondSection :links="links"/>
    <MyterzaSection :cards="cards"/>
    <MyquartaSection :teams="teams"/>

  </div>
</template>

<script>
import MyprimSection from '@/components/MyprimSection.vue';
import MysecondSection from'@/components/MysecondSection.vue'
import MyterzaSection from '@/components/MyterzaSection.vue' 
import MyquartaSection from '@/components/MyquartaSection.vue' 


  export default {
      name:'MyMain',
      components:{
        MyprimSection,
        MysecondSection,
        MyterzaSection,
        MyquartaSection
      },
       props:{
        links:Array,
        cards:Array,
        teams:Array
    }
  };

</script>
 

<style lang="scss">
</style >