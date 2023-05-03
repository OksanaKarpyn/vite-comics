<script>
import HeaderNav from './components/HeaderNav.vue';
import MainHeaderContent from './components/MainHeaderContent.vue';
import MainHeaderNav from './components/MainHeaderNav.vue';
import MainContent from './components/MainContent.vue';
export default {
  name: 'AppVue',
  components: {
    HeaderNav,
    MainHeaderContent,
    MainHeaderNav,
    MainContent,
  }
}

</script>

<template>
  <HeaderNav></HeaderNav>
  <MainHeaderContent></MainHeaderContent>
  <MainHeaderNav></MainHeaderNav>
  <h1>ciao</h1>
</template>

<style lang="scss" >
@use './style/main.scss' as *;
</style>
