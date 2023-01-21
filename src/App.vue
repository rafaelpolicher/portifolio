<template>
  <Navbar/>
  <Home/>
  <About/>
  <Knowledge/>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue'
import About from './components/About.vue';
import Knowledge from './components/Knowledge.vue';

export default{
  components:{
    Navbar,
    Home,
    About,
    Knowledge
}
}
</script>
<style scoped>

</style>
