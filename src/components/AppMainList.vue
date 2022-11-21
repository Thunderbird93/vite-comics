<script>
export default {
    name: 'AppMainList',
    props:{
        cards: Object
    },
    data(){
        return{
        }
    }
}
</script>

<template>
  <div class="lista">
    <div class="container">
        <div v-for="(card, index) in cards" class="card">
            <img :src="card.thumb" :alt="card.series">
            <h5>{{card.series}}</h5>
        </div>
    </div>
  </div>      
</template>

<style lang="scss" scoped>
    @use '../style/partial/mixin' as *;
    @use '../style/partial/variables' as *;

 .lista{
    background-color: #1C1C1C;
    min-height: 400px;
    max-height: 100vh;
    .container{
        min-height: 400px;
        .card{
            height: 150px;
            width: 150px;
        }
    }
 }

</style>