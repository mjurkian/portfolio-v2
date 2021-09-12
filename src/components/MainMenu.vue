<template>
  <nav>
    <div class="menu-item"><a href="#">Home</a></div>
    <div class="menu-item"><a href="#">About</a></div>
    <div class="menu-item"><a href="#">Experience</a></div>
    <div class="menu-item"><a href="#">Contact</a></div>
  </nav>
</template>

<script>
export default {
  name: "MainMenu"
}
</script>

<style scoped>
nav {
  display: flex;
  justify-content: flex-end;
  align-items: center;
  height: 90px;
  background: bisque;

}
</style>
