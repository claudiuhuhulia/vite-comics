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

li {
  list-style-type: none;
}



/* utilities */
.container {
  margin: 0 auto;
  max-width: 1200px;
}
</style>