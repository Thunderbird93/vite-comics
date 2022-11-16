<script>

import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import links from './data/menu/menu';
import icons from './data/social/social';

export default {
  name: 'App',
  components:{
    AppHeader,
    AppFooter,
    AppMain
  },
  data(){
    return{
      links,
      icons
    }
  }
}
</script>

<template>

  <AppHeader :menu="links" />
  <AppMain />
  <AppFooter :social="icons" />

</template>

<style lang="scss">
  @use './style/general.scss'
</style>