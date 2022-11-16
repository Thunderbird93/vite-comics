<script>

import AppHeader from './components/AppHeader.vue';
import AppFooter from './components/AppFooter.vue';
import AppMain from './components/AppMain.vue';
import links from './data/menu';

export default {
  name: 'App',
  components:{
    AppHeader,
    AppFooter,
    AppMain
  },
  data(){
    return{
      links
    }
  }
}
</script>

<template>

  <AppHeader :menu="links" />
  <AppMain />
  <AppFooter />

</template>

<style lang="scss">
  @use './style/general.scss'
</style>