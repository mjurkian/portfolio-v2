<template>
  <header>
    <Hero/>
  </header>
  <main>
    <Sidebar/>
    <About/>
    <Skills/>
    <Projects/>
    <Contact/>
  </main>
  <footer>
    <Footer />
  </footer>
</template>

<script>
import Sidebar from '@/components/sidebar/Sidebar.vue'
import Hero from '@/components/Hero'
import About from '@/components/About.vue'
import Skills from "@/components/Skills"
import Projects from "@/components/Projects"
import Contact from "@/components/Contact"
import Footer from "@/components/Footer"

export default {
  name: 'App',
  components: {
    Sidebar,
    Hero,
    About,
    Skills,
    Projects,
    Contact,
    Footer
  }
}
</script>
