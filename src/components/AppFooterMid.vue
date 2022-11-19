<script>
export default {
    name: 'AppFooterMid',
    data(){
        return
    }
}
</script>


<template>
<div class="mid-foot">

    <div class="container">
        <div class="f-menu"></div>
        <div class="f-logo"></div>
    </div>
</div>  
    </template>


<style lang="scss" scoped>
@use '../style/partial/mixin' as *;
@use '../style/partial/variables' as *;

.mid-foot{
background-image: url(../assets/img/footer-bg.jpg);
height: 370px;
}
</style>