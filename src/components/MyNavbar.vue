<template>
  <nav>
     <span class="icone">
        <i class="fa-regular fa-clock"></i>
        Open Hours: Mon-Sat-9:00-18:00
     </span>
    
    <span>
        <i class="fa-solid fa-phone-flip"></i>
        +(305)123-65678
    </span>

    <i class="fa-regular fa-envelope"></i>
     hello@example.com
     
    <i class="fa-brands fa-square-facebook"></i>
    <i class="fa-brands fa-twitter"></i>
    <i class="fa-brands fa-linkedin"></i>
  </nav>
</template>

<script>
export default {
    name:'MyNavbar'
}
</script>

<style lang="scss">
nav{
    height: 30px;
    color: #bcbddb;
    background-color:rgb(33, 51, 62) ;
    line-height: 30px;
    padding: 0.5rem 0 ;
    
    span.icone{
        margin-left:10rem;
        margin-right:2rem;

    }
    .fa-brands{
        margin-left:2rem;
        
        
    }
}


</style>