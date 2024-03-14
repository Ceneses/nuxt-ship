<template>
<main class="grid grid-cols-2 p-2">
  <div class="p-24">
    <h1 class="pt-10 text-3xl font-serif">Marketing Website done with Nuxt!</h1>
    <p class="pt-4 font-serif">
      NuxtShip is a starter template for startups, marketing websites & landing pages.
      It is built with <a href="https://nuxtjs.org/">Nuxt.js</a>
    </p>
    <div class="mt-10 flex flex-row gap-x-4 font-serif">
      <button class="px-5 py-2 rounded-md bg-blue-300">Get Started</button>
      <button class="px-5 py-2 rounded-md border-2 border-blue-300 hover:bg-blue-300">View Repo</button>
    </div>
  </div>
  <div class="p-24">
    <img src="@/assets/img/hero.jpg" alt="hero" class="transition-transform transform rounded-full hover:scale-125" width="512" height="512">
  </div>
</main>
</template>

<script>
export default {
  name: "Hero"
};
</script>

<style scoped>

</style>