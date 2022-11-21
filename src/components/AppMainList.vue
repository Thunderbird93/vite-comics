<script>
export default {
    name: 'AppMainList',
    data(){
        return{
        }
    }
}
</script>

<template>
  <div class="lista">
    <div class="container">

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
    }
 }

</style>