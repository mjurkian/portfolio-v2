<template>
  <section id="hero" class="flex relative items-center justify-center max-w-screen-lg min-h-screen mx-auto">
      <div class="container flex  flex-col-reverse lg:flex-row items-center gap-12 md:mx-auto">
        <div class="flex justify-center flex-1 md:order-1 mb-10 md:mb-16 lg:mb-0 z-10">
          <img src="../assets/mj-min.jpg" alt="" class="w-5/6 h-5/6 sm:3/4 rounded-3xl shadow-2xl">
        </div>
        <div class="flex flex-1 flex-col items-center lg:items-start">
          <h1 class="mb-8 text-4xl md:text-7xl text-mj-php-mellow">Hi, I'm Michal</h1>
          <p class="text-mj-lavender">Lorem ipsum dolor sit amet consectetur adipisicing elit. Sint reprehenderit autem ratione vero illo, ut maiores expedita, itaque accusantium saepe molestias laborum consequatur nulla voluptatibus vel voluptate laboriosam ex quod alias sed sunt totam ullam! Distinctio alias totam corporis dolores ex, sapiente provident voluptatem ea voluptas, omnis blanditiis molestiae veritatis possimus odio in eaque ad mollitia quam. Blanditiis, corrupti at!</p>
        </div>
      </div>
  </section>
</template>

<script>
export default {
    name: 'Hero',
}
</script>
