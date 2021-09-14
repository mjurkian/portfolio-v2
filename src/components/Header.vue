<template>
  <header class="fixed flex w-full items-center font-mono px-4 ">
    <!-- <img class="h-28 m-2" src="../assets/logo.png" alt="Logo MJ"> -->
    <p class="font-serif text-8xl text-gray-200 ml-10">mj</p>

    <nav class="flex-1 mr-10">
      <ul class="hidden sm:flex justify-end items-center gap-5 text-gray-200 text-base">
        <li><a href="/#hero" class="rounded-md focus:ring-2 py-2 px-4">Home</a></li>
        <li><a href="/#about" class="rounded-md focus:ring-2 py-2 px-4">About</a></li>
        <li><a href="/#experience" class="rounded-md focus:ring-2 py-2 px-4">Experience</a></li>
        <li><a href="/#contact" class="rounded-md focus:ring-2 py-2 px-4">Contact</a></li>
        <li><button type="button" class="bg-indigo-700 hover:bg-indigo-900 py-2 px-4 rounded-md shadow-sm transition delay-100 duration-100 ease-linear">Resume</button></li>
      </ul>
    </nav>

    <div class="flex sm:hidden flex-1 justify-end">
      <MenuIcon class="h-8 w-8 text-blue-800"/>
    </div>
  </header>
</template>

<script>
import { MenuIcon } from '@heroicons/vue/solid'

export default {
  name: 'Header',
  components: {
    MenuIcon,
  }
}
</script>
