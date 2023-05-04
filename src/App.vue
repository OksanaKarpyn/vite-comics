<script>
import HeaderNav from './components/HeaderNav.vue';
import MainHeader from './components/MainHeader.vue';
import MainHeaderNav from './components/MainHeaderNav.vue';
import MainContent from './components/MainContent.vue';
import FooterComp from './components/FooterComp.vue';
export default {
  name: 'AppVue',
  components: {
    HeaderNav,
    MainHeader,
    MainHeaderNav,
    MainContent,
    FooterComp,
  }
}

</script>

<template>
  <header>
    <HeaderNav></HeaderNav>
  </header>
  <main>
    <MainHeader></MainHeader>
    <MainHeaderNav></MainHeaderNav>
    <MainContent></MainContent>
  </main>
  <footer>
    <FooterComp></FooterComp>
  </footer>
</template>

<style lang="scss" >
@use './style/main.scss' as *;
</style>
