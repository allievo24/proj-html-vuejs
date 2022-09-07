<template>
  <section class="quarta">
    
    <div class="containerCard">
      <div
        class="card"
        v-for="(person, index) in teams"
        :key="index"
        :teams="teams"
      >
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
          <img src="@/assets/img/team-1.jpg" alt="" />
        </div>
        <div class="info">
          <h4>{{ person.nome }}</h4>
          <span class="job">{{ person.job }}</span>
          
          <div class="containerIcone">
            <div class="icone">
              <span>
                <i class="fa-brands fa-square-facebook"></i>
              </span>
            </div>
            <div class="icone">
              <span>
                <i class="fa-brands fa-twitter"></i>
              </span>
            </div>
            <div class="icone">
              <span>
                <i class="fa-brands fa-linkedin"></i>
              </span>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="text">
      <h3>President Speech</h3>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Est, a labore.</p>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Est, a labore.</p>
      <p>Lorem ipsum dolor sit, amet consectetur adipisicing elit. Est, a labore.</p>
       <div class="ceo">
         T.JOHNSON
       </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MyquartaSection",
  props: {
    teams: Array,
  },
};
</script>

<style lang="scss">

.quarta {
  display: flex;
  .text{
    background:  rgb(5, 130, 131);
    padding: 2rem;
    width: 20%;
    margin: auto;
    border-radius: 10px;
    color:white;

   p{
    margin-top: 20px;
   }
    .ceo{
      margin-top: 2rem;
    }
  }
  .containerCard {
    width: 60%;
    display: flex;
    flex-wrap: wrap;
    margin: auto;
    border: 2px solid rgb(38, 0, 255);
    .containerIcone {
      display: flex;
    }

    .card {
      width: calc(80% / 2 - 1rem);
      //border: 2px solid green;
      display: flex;
      margin: auto;
      img {
          width: 150px;
          height: 200px;

          }
    
        .info {
        // border: 2px solid rgb(255, 187, 0);
         padding-bottom:2rem;
        
         .job,h4{
          display: block;
          margin-top: 1rem;
         // border: 2px solid red;
          padding-left:1rem ;
         }
         .job{
          font-size: 13px;
          color:rgb(85, 108, 134);
         }
         h4{
          font-size: 20px;
         }

      .icone {
        width: 40px;
        height: 40px;
        background: rgb(218, 236, 237);
        border-radius: 50%;
        margin: 3rem 1rem 1rem 1rem;
        // border: 2px solid red;

        span {
          display: inline-block;
          width: 35px;
          color: rgb(0, 128, 129);
          font-size: 25px;
          text-align: center;
          transform: translatey(20%);
        }
      }
    }
    
    
    }

    
  }
}


</style>