<script>
export default {
    name: 'AppFooterTop',
    props:{
        prodotti: Array
    },
    data(){
        return{
        }
    }
}

</script>

<template>
  <div class="merch">
    <div class="container">
        <ul class="merch-list">
            <li v-for="(prodotto, index) in prodotti" :key="index" class="merch-box">
                <a href="#">
                    <img :src="prodotto.img" alt="">
                    <h3>{{prodotto.titolo}}</h3>
                </a>
            </li>
        </ul>
    </div>
  </div>
</template>

<style lang="scss" scoped>
@use '../style/partial/variables' as *;
@use '../style/partial/mixin' as *;

.merch{
    background-color: $primary-color;
    height: 110px;
    .container{
        .merch-list{
            display: flex;
            .merch-box{
                max-width: 20%;
                a{
                display: flex;
                align-items: center;
                img{
                    height: 50px;
                }
                }
            }
        }    
    }
}

</style>