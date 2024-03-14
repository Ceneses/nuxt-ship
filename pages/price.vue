<template>
  <div class="flex flex-row gap-x-4 items-center justify-center w-fit mx-auto">
    <div class="mt-4 ml-4 w-fit px-10 py-6 border-slate-600 border-2 rounded-md" v-for="item in plan" :key="item">
      <h4 class="text-dark-400 font-serif">{{item.title}}</h4>
      <p class="text-4xl font-serif mt-4">{{item.price}}</p>
      <ul class="mt-4">
        <li v-for="param in item.features" :key="param" class="flex items-start gap-3 text-gray-800 font-serif">
          <Icon name="simple-icons:vercel"></Icon>
          {{param}}
        </li>
      </ul>
      <button class="mt-4 px-12 py-2 rounded-md font-serif border-slate border-2">{{item.button.text}}</button>
    </div>
  </div>
</template>

<script setup>
definePageMeta({
  layout: "landing"
})
const plan = [
  {
    title: "Personal",
    price: "Free",
    features: [
      "LifeTime free",
      "Up to 3 users",
      "Unlimited Pages",
      "Nuxt Sub domains",
      "Nuxt Sub domains",
      "Nuxt Sub domains"
    ],
    button: {
      text: "Get Started",
      link: "#"
    }
  },
  {
    title: "StartUp",
    price: "$19",
    features: [
      "Unlimited users",
      "Unlimited Pages",
      "Nuxt Sub domains",
      "Unlimited Domains",
      "Unlimited SSL Certificates",
      "Unlimited API Requests"
    ],
    button: {
      text: "Get Started",
      link: "#"
    }
  },
  {
    title: "Popular",
    popular: true,
    price: "Custom",
    features: [
      "All Pro Features",
      "Unlimited Custom domains",
      "99.99% Uptime SLA",
      "SAML & SSO Integration",
      "Dedicated Account Manager",
      "24/7 Phone Support"
    ],
    button: {
      text: "Buy It",
      link: "#"
    }
  }
];
</script>

<style scoped>

</style>