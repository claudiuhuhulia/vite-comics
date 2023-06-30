<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';
import FooterUser from './components/FooterUser.vue';



export default {
  name: 'Comics',
  components: { AppHeader, AppMain, AppFooter, FooterUser },
  data() {
    return {

    }
  }
}
</script>

<template>
  <AppHeader />
  <AppMain />
  <AppFooter />
  <FooterUser />
</template>


<style lang="scss">
@use './assets/scss/style.scss'
</style>