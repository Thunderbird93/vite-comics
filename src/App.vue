<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import AppFooterMid from './components/AppFooterMid.vue';
import links from './data/menu/menu.js';
import icons from './data/social/social.js';
import imenu from './data/menu/fmenu.js';

export default {
  name: 'App',
  components:{
    AppHeader,
    AppFooter,
    AppMain,
    AppFooterMid
  },
  data(){
    return{
      links,
      icons,
      imenu
    }
  }
}
</script>

<template>

  <AppHeader :menu="links" />
  <AppMain />
  <AppFooterMid :fmenu="imenu"/>
  <AppFooter :social="icons" />

</template>

<style lang="scss">
  @use './style/general.scss'
</style>