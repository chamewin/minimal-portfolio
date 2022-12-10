<script setup lang="ts">
  import intro from '../data/intro'
</script>

<template>
  <div className="flex items-center justify-center flex-col text-center pt-20 pb-6">
    <h1 className="text-4xl md:text-7x">{{ intro.name }}</h1>
    <p className="text-base md:text-xl mb-3 font-medium">{{ intro.title }}</p>
    <p className="text-sm max-w-xl mb-6 font-bold">{{ intro.bio }}</p>
  </div>
</template>
