<template>
  <MainMenu />
  <img alt="Vue logo" src="./assets/logo.png">
  <router-view />
</template>

<script>
import MainMenu from './components/MainMenu'

export default {
  name: 'App',
  components: {
    MainMenu
  }
}
</script>

<style>

</style>
