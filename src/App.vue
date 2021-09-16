<template>
  <Sidebar />
  <Hero />
  <About />
  <Skills />
  <Projects />
  <Contact />
</template>

<script>
import Sidebar from '@/components/sidebar/Sidebar.vue'
import Hero from  '@/components/Hero'
import About from '@/components/About.vue'
import Skills from "@/components/Skills";
import Projects from "@/components/Projects";
import Contact from "@/components/Contact";

export default {
  name: 'App',
  components: {
    Sidebar,
    Hero,
    About,
    Skills,
    Projects,
    Contact
  }
}
</script>
