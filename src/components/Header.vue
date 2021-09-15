<template>
  <header class="fixed flex items-center w-full px-4 font-mono ">
    <!-- <img class="m-2 h-28" src="../assets/logo.png" alt="Logo MJ"> -->
    <p class="ml-10 font-serif font-thin text-mj-lavender text-8xl">mj</p>

    <nav :class="menuOpen ? 'block': 'hidden'" class="w-full mr-10 md:w-auto md:flex-1 md:block" >
      <ul class="items-center justify-end gap-5 text-base text-mj-lavender md:flex">
        <li><a href="/#hero" class="px-4 py-2 rounded-md focus:ring-2">Home</a></li>
        <li><a href="/#about" class="px-4 py-2 rounded-md focus:ring-2">About</a></li>
        <li><a href="/#experience" class="px-4 py-2 rounded-md focus:ring-2">Experience</a></li>
        <li><a href="/#contact" class="px-4 py-2 rounded-md focus:ring-2">Contact</a></li>
        <li><button type="button" class="btn btn-green">Resume</button></li>
      </ul>
    </nav>

    <div class="flex justify-end flex-1 w-8 h-8 md:hidden ">
      <MenuIcon @click="toggle" class="w-8 h-8 cursor-pointer text-mj-mellow"/>
    </div>
  </header>
</template>

<script>
import { MenuIcon } from '@heroicons/vue/solid'

export default {
  name: 'Header',
  components: {
    MenuIcon,
  },
  data() {
    return {
    menuOpen: false
    }
  },
  methods: {
    toggle() {
      this.menuOpen = !this.menuOpen
    }
  }
}
</script>
