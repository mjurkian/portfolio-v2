<template>
  <div class="fixed top-0 bottom-0 left-0 z-10 p-2 transition text-mj-lavender bg-mj-burgundy" :style="{ width: sidebarWidth }">
    <h2 class="mb-10 text-center">
      <span v-if="collapsed">mj</span>
      <span v-else class="text-5xl text-center">-mj-</span>
    </h2>

    <nav class="overflow-hidden">
      <ul class="gap-5">
        <li>
          <a :to="to" class="flex items-center mb-5" :class="{ active: isActive }" href="#hero">
            <HomeIcon class="w-7 h-7 text-mj-lavender" />
            <span class="ml-3" v-if="!collapsed">Home</span>
          </a>
        </li>
        <li>
          <a :to="to" class="flex items-center mb-5" :class="{ active: isActive }" href="#about">
            <UserIcon class="w-7 h-7 text-mj-lavender" />
            <span class="ml-3" v-if="!collapsed">About</span>
          </a>
        </li>
        <li>
          <a :to="to" class="flex items-center mb-5" :class="{ active: isActive }" href="#experience">
            <DesktopComputerIcon class="w-7 h-7 text-mj-lavender" />
            <span class="ml-3" v-if="!collapsed">Experience</span>
          </a>
        </li>
        <li>
          <a :to="to" class="flex items-center mb-5" :class="{ active: isActive }" href="#contact">
            <PhoneIcon class="w-7 h-7 text-mj-lavender" /> 
            <span class="ml-3" v-if="!collapsed">Contact</span>
          </a>
        </li>
      </ul>
    </nav>

    <span @click="toggleSidebar">
      <ArrowSmLeftIcon class="absolute w-8 h-8 transition duration-300 transform right-1 bottom-4 text-mj-lavender" :class="{ 'rotate-180': collapsed }" />
    </span>
  </div>

  <div class="absolute top-5 right-5 md:hidden">
      <MenuIcon @click="toggle" class="w-8 h-8 cursor-pointer text-mj-burgundy"/>
  </div>
</template>

<script>
import { collapsed, toggleSidebar, sidebarWidth } from "@/components/sidebar/state";
import { HomeIcon, UserIcon, DesktopComputerIcon, PhoneIcon, ArrowSmLeftIcon, MenuIcon } from '@heroicons/vue/outline'


export default {
  name: "Sidebar",
  props: {},
  components: { 
    HomeIcon,
    UserIcon,
    DesktopComputerIcon,
    PhoneIcon,
    ArrowSmLeftIcon,
    MenuIcon
  },
  setup() {
    return { collapsed, toggleSidebar, sidebarWidth }
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