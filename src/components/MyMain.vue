<template>
  <div>
    <MyprimSection/>
    <MysecondSection/>
    <MyterzaSection/>
    <MyquartaSection/>

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
      }
  };

</script>

<style>
</style>