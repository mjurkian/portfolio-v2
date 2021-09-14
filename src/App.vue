<template>
  <Header />
  <Hero />
  <About />
</template>

<script>
import Header from './components/Header'
import Hero from  './components/Hero'
import About from './components/About.vue'

export default {
  name: 'App',
  components: {
    Header,
    Hero,
    About
  }
}
</script>
