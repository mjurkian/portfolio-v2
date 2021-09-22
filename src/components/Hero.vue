<template>
  <section id="hero" class="flex relative items-center justify-center max-w-screen-lg min-h-screen mx-auto">
    <div class="container flex flex-col-reverse lg:flex-row items-center gap-12 md:mx-auto">
      <div class="flex justify-center flex-1 lg:order-1 mb-10 md:mb-16 lg:mb-0 z-10">
        <img alt="" class="w-5/6 h-5/6 sm:3/4 rounded-3xl shadow-2xl" src="../assets/cat-min.jpg">
      </div>
      <div class="flex flex-1 flex-col items-center lg:items-start">
        <h1 class="mb-8 text-4xl md:text-7xl text-mj-php-mellow">Hi, I'm Michal</h1>
        <p class="text-mj-lavender text-2xl">a Husband, a Father, a Web Developer.</p>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Hero',
}
</script>
