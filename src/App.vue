<template>
  <Sidebar />
  <!-- <Header /> -->
  <Hero />
  <About />
</template>

<script>
import Sidebar from './components/sidebar/Sidebar.vue'
// import Header from './components/Header'
import Hero from  './components/Hero'
import About from './components/About.vue'

export default {
  name: 'App',
  components: {
    Sidebar,
    // Header,
    Hero,
    About
  }
}
</script>
