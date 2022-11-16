<script>
export default {
    name: 'AppFooter'
}
</script>

<template>
  <footer>
    <div class="container">
      <div class="cta">
        <p>SIGN-UP NOW!</p>
      </div>
      <div class="social">
        <p>FOLLOW US</p>
        <img src="../assets/img/footer-facebook.png" alt="">
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
  }
}
  
</style>