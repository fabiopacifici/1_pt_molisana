<script>
/* 1. Import the components */
import AppHeaderVue from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';



export default {
  name: 'App',
  /* 2. Register your components here */
  components: {
    AppHeaderVue,
    AppMain,
    AppFooter
  }
}
</script>

<template>
  <!-- User it -->
  <AppHeaderVue></AppHeaderVue>
  <AppMain></AppMain>
  <AppFooter></AppFooter>

</template>