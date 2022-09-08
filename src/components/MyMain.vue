<template>
  <div>
    <MyprimSection/>
    <MysecondSection :links="links"/>
    <MyterzaSection :cards="cards"/>
    <MyquartaSection :teams="teams"/>
    <MyquintaSection :News="News"/>

  </div>
</template>

<script>
import MyprimSection from '@/components/MyprimSection.vue';
import MysecondSection from'@/components/MysecondSection.vue'
import MyterzaSection from '@/components/MyterzaSection.vue' 
import MyquartaSection from '@/components/MyquartaSection.vue' 
import MyquintaSection from '@/components/MyquintaSection.vue' 



  export default {
      name:'MyMain',
      components:{
        MyprimSection,
        MysecondSection,
        MyterzaSection,
        MyquartaSection,
        MyquintaSection
      },
       props:{
        links:Array,
        cards:Array,
        teams:Array,
        News:Array
    }
  };

</script>
 

<style lang="scss">
</style >