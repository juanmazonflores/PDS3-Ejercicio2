<template>
  <Navbar/>
  <Home/>
  <Acerca/>
  <Habilidades/>
  <Proyectos/>
  <Footer/>
  <BotonArriba/>
</template>

<script>
  import Navbar from './components/Navbar.vue'
  import Home from './components/Home.vue'
  import Acerca from './components/Acerca.vue'
  import Habilidades from './components/Habilidades.vue'
  import Proyectos from './components/Proyectos.vue'
  import Footer from './components/Footer.vue'
  import BotonArriba from './components/BotonArriba.vue'

export default {
  name: 'App',
  components: {
    Navbar,
    Home,
    Acerca,
    Habilidades,
    Proyectos,
    Footer,
    BotonArriba
  }
}
</script>

<style>
  @import "../public/css/style.css";
</style>
