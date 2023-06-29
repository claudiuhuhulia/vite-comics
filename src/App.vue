<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';


export default {
  name: 'Comics',
  components: { AppHeader, AppMain, AppFooter },
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
</template>


<style>
/* reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* generics */
img {
  max-width: 80%;
  height: auto;
}

body {
  font-family: Condensed, Open Sans;
}

a {
  text-decoration: none;
}

/* utilities */
.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>