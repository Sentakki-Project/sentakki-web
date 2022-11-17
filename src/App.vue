<template>
    <NavbarVue/>
    <router-view/>
</template>

<script>
import NavbarVue from './components/Navbar.vue';
export default {
  name: 'App',
  components:{NavbarVue},
  data(){
    return{
      items:[
        {title:'O projekcie',},
        {title:'Team'}
      ],
    }
  },
}
</script>
<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body{
  background: #eee;
}
</style>
