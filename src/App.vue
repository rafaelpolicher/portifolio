<template>
  <Navbar/>
  <Home/>
  <About/>
  <Knowledge/>
  <Projects/>
  <Contact/>
</template>

<script>
import Navbar from './components/Navbar.vue';
import Home from './components/Home.vue'
import About from './components/About.vue';
import Knowledge from './components/Knowledge.vue';
import Projects from './components/Projects.vue';
import Contact from './components/Contact.vue';

export default{
  components:{
    Navbar,
    Home,
    About,
    Knowledge,
    Projects,
    Contact
}
}
</script>
<style scoped>

</style>
