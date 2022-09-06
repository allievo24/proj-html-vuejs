<template>
    <section class="seconda" >
        <div class="container" v-for="(link ,index) in links" :key="index" :links="links">
            <span>{{links.t1}}</span>
            <h2>{{link.t2}}</h2>
            <ul>
                <li>
                    <a :href="link.url">{{link.text}}</a>
                    {{linkS.number}}
                </li>
            </ul>
        </div>

    </section>
</template>

<script>
export default {
    name :'MysecondSection',
    props:{
        links:Array
    }
  
}
</script>

<style lang="scss">
  .seconda{
    height: 500px;
    border: 2px solid black;
    .container{
        background: blue;
    }
  }

   

</style>