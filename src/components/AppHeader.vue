<script>
export default {
  name: 'AppHeader',
  props:{
    menu: Array
  },
  data(){
    return{
    }
  }
}
</script>


<template>
    <header>
        <div class="container">
            <div class="logo">
                <img src="/dc-logo.png" alt="logo">
            </div>
            
            <nav class="menu">
                    <ul>
                        <li v-for="(link, index) in menu" :key="index">
                            <a :class="{'active': link.current}" :href="link.href">
                                {{link.text}} 
                            </a>
                        </li>
                     </ul>
            </nav>
        </div>    
    </header>
</template>

<style lang="scss" scoped>

@use '../style/partial/mixin' as *;
@use '../style/partial/variables' as *;

    header{
        background-color: white;
        .container{
        height: 120px;
      .menu{
        height: 100%;
        ul {
        display: flex;
        height: 100%;
        li {
         display: flex;
         align-items: center;
         margin: 0 10px;
         list-style: none; 
         height: 100%;
         //debug
        border: 1px dotted red;
         a {
            text-decoration: none;
            color: black;
            font-weight: 600;
            border-bottom: 5px solid rgba(255, 255, 255, 0);
          }
        }
        
        li:hover{
            border-bottom: 5px solid $primary-color;
            a{
            color: $primary-color;
            }
        }
      }
      }
    }
    }

</style>