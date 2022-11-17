<script>
export default {
    name: 'AppFooter',
    props:{
      social: Array
    },
    data(){
      return{
    }
  }
}
</script>

<template>
  <footer>
    <div class="container">
      <div class="cta">
        <p>SIGN-UP NOW!</p>
      </div>
      <div class="social">
        <ul>
          <p>FOLLOW US</p>
          <li v-for="(icon, index) in social" :key="index">
            <img :src="icon.path" alt="">
          </li>
        </ul>
      </div>
    </div>
  </footer>
</template>

<style lang="scss" scoped>
@use '../style/partial/mixin' as *;
@use '../style/partial/variables' as *;
footer{
  background-color: #303030;
  .container{
    height: 120px;
    //debug
    border: 1px dotted red;
    .social{
      display: flex;
      ul{
        display: flex;
        li{
          list-style: none; 
        }
      }
    }
  }
}
  
</style>