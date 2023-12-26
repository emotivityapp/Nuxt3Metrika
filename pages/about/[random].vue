<template>
  <h1>Random Page is: {{ route.params.random }}</h1>

  <NuxtLink to="/">
        To main page
  </NuxtLink>
</template>

<script setup>
const route = useRoute()
</script>