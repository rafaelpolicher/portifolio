<template>
  <Navbar/>
  <Home/>
  <About/>
  <Knowledge/>
  <Projects/>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue'
import About from './components/About.vue';
import Knowledge from './components/Knowledge.vue';
import Projects from './components/Projects.vue';

export default{
  components:{
    Navbar,
    Home,
    About,
    Knowledge,
    Projects
}
}
</script>
<style scoped>

</style>
