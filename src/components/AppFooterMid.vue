<script>
export default {
    name: 'AppFooterMid',
    props:{
        fmenu: Object
    },
    data(){
        return
    }
}
</script>


<template>
<div class="mid-foot">

    <div class="container">
        <div class="f-menu">
            <ul class="first-ul">
                <li class="first-li" v-for="(ilmenu, index) in fmenu" :key="index">
                    <h3>{{ilmenu.titolo}}</h3>
                    <ul>
                        <li v-for="(voce, index) in ilmenu.voci" :key="index">
                            <a href="#">{{ilmenu.voci[index]}}</a>
                        </li>
                    </ul>
                </li>
            </ul>
        </div>
        <div class="f-logo"></div>
    </div>
</div>  
    </template>


<style lang="scss" scoped>
@use '../style/partial/mixin' as *;
@use '../style/partial/variables' as *;

.mid-foot{
background-image: url(../assets/img/footer-bg.jpg);
height: 280px;
padding: 20px 0;
    h3{
        color: white;
    }
    .container{
        align-self: start;
            .f-menu{
                height: 100%;
                display: flex;
                .first-ul{
                    display: flex;
                    flex-direction: column;
                    column-count: auto;
                    column-gap: 30px;
                    column-width: 300px;
                    flex-wrap: wrap;
              .first-li {
                display: flex;
                flex-direction: column;
                a{
                    color: #535D65;
                }
             }
          }
        }
    }        
}

</style>