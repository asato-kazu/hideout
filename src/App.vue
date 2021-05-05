<template>
  <v-app>
    <v-main>
      <NaviCom></NaviCom>
      <router-view/>
      
    </v-main>
  </v-app>
</template>

<script>
import NaviCom from './components/Navi'

export default {
  name: 'App',
  components: {
    NaviCom,
  },
  data: () => ({
    //
  }),
};
</script>
