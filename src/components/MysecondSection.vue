<template>
  <section class="seconda">
    <div class="titolo">
      <span>WHAT ARE WE DOING</span>
      <h2>Results in Numners</h2>
    </div>
    <div
      class="container"
      v-for="(link, index) in links"
      :key="index"
      :links="links"
    >
      <div class="link">
        <div>{{ link.number }}</div>

        <span
          ><a :href="link.url">{{ link.text }}</a></span
        >
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: "MysecondSection",
  props: {
    links: Array,
  },
};
</script>

<style lang="scss">
.seconda {
  border: 2px solid red;
      display: flex;
      flex-wrap: wrap;
      text-align: center;
      justify-content:space-around;
      padding: 2rem;



  .container {
    border: 2px solid yellow;
    text-align: center;
    

    

   
    .link {
      border: 2px solid;
      text-align: center;

    }
  }
  .titolo {
    border: 2px solid green;
     width: 100%;
  }
}
</style>