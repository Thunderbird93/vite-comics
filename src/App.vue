<script>
import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import AppFooterMid from './components/AppFooterMid.vue';
import AppFooterTop from './components/AppFooterTop.vue';
import AppMainList from './components/AppMainList.vue'
import links from './data/menu/menu.js';
import icons from './data/social/social.js';
import imenu from './data/menu/fmenu.js';
import prodotti from './data/merch/prodotti';

export default {
  name: 'App',
  components:{
    AppHeader,
    AppFooter,
    AppMain,
    AppMainList,
    AppFooterMid,
    AppFooterTop
  },
  data(){
    return{
      links,
      icons,
      imenu,
      prodotti
    }
  }
}
</script>

<template>

  <AppHeader :menu="links" />
  <AppMain />
  <AppMainList />
  <AppFooterTop :prodotti="prodotti" />
  <AppFooterMid :fmenu="imenu"/>
  <AppFooter :social="icons" />

</template>

<style lang="scss">
  @use './style/general.scss'
</style>