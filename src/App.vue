<template>
  <v-app>
    <navbar></navbar>
    <admin></admin> 
   <!--  <HelloWorld></HelloWorld> -->
  </v-app>
</template>



<script>
import admin from './components/admin';
/* import HelloWorld from './components/HelloWorld'; */
import navbar from './components/navbar';
export default {
  name: 'App',
  components: {
    admin,
    /* HelloWorld, */
    navbar,
  },
  data: () => ({
    //
  }),
};
</script>
