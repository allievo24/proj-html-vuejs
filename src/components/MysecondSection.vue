<template>
    <section class="seconda" >
        <div class="container" v-for="(link ,index) in links" :key="index">
            <span>{{link.t1}}</span>
            <h2>{{link.t2}}</h2>
            <ul>
                <li>
                    <a :href="link.url">{{link.text}}</a>
                    {{link.number}}
                </li>
            </ul>
        </div>

    </section>
</template>

<script>
export default {
    name :'MysecondSection',
    data(){
        return{
           links:[
              {
                t1:'WHAT ARE WE DOING',
                t2:'Results in Numners'
              },
             {
               text:'Certification',
               number:'120', 
               url:'#'

             },
              {
               text:'Employees',
               number:'230', 
               url:'#'

             },
              {
               text:'Custromers',
               number:'517', 
               url:'#'

             },
             {
               text:'Countries Served',
               number:'94', 
               url:'#'

             },
           ] 
        }
    }
}
</script>

<style lang="scss">
   

</style>