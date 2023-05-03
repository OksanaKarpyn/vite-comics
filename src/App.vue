<script>
import HeaderNav from './components/HeaderNav.vue';
import MainHeaderContent from './components/MainHeaderContent.vue';
import MainHeaderNav from './components/MainHeaderNav.vue';
import MainContent from './components/MainContent.vue';
import Footer from './components/Footer.vue';
export default {
  name: 'AppVue',
  components: {
    HeaderNav,
    MainHeaderContent,
    MainHeaderNav,
    MainContent,
    Footer,
  }
}

</script>

<template>
  <HeaderNav></HeaderNav>
  <MainHeaderContent></MainHeaderContent>
  <MainHeaderNav></MainHeaderNav>
  <MainContent></MainContent>
  <Footer></Footer>
</template>

<style lang="scss" >
@use './style/main.scss' as *;
</style>
