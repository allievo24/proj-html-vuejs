<template>
 <section class="prima">
    <span>INTRODUCTION VIDEO</span>
    <h1>Advisory <span class="titolo">Performance </span></h1>
    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Eligendi quasi, quae nostrum tempore atque mollitia? Lorem ipsum, dolor sit amet consectetur adipisicing elit. Dicta, minima.</p>
    <div class="video">
        <img src="@/assets/img/video-1.jpg" alt="">
    </div>
 </section>
   

    
</template>

<script>
export default {
 name:'MyprimSection'
}
</script>

<style lang="scss">
 .prima{
    text-align: center;
    width: 70%;
    margin:auto;
    img{
        width: 100%;
        
    }
    .titolo{
            color:rgb(6, 244, 244);
            background-color:rgb(218, 236, 237);
            border-radius: 3px;
            padding: 0 0.5rem;
            
    }
    p{
        padding: 0 2rem;
    }
   
 }


</style>