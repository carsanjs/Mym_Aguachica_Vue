<script>
import IndexNav from './components/NavP.vue';
import IndexFooter from './components/FooterT.vue';
import IndexMenu from './components/DivMenus/Menu.vue'
export default {
  name: 'App',
data() {
  return {
  }
},
components:{
  IndexNav,
  IndexFooter,
  IndexMenu
}
}
</script>

<template>
<IndexNav></IndexNav>
<div>
  <IndexMenu></IndexMenu>
</div>

  <v-app>
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
  <IndexFooter></IndexFooter>
</template>
