<template>
<div :class="['mt-16', align === 'center' && 'text-center']">
  <h1 class="text-4l lg:text-5xl font-bold lg:tracking-tight">
    <slot name="title">Title</slot>
  </h1>
  <p class="text-lg mt-4 text-slate-600">
    <slot name="desc">Some Description</slot>
  </p>
</div>
</template>

<script setup lang="ts">
defineProps({
  align: {
    type: String,
    default: 'center'
  }
})
</script>

<style scoped>

</style>