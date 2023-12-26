<template>

  <h1>Page One Link: </h1>
  <NuxtLink :to="`/about/${getRandomInt(1, 10)}`">
        about link
  </NuxtLink>

  <h2>Page Two Link: </h2>
  <NuxtLink to="/contacts">
        contacts link
  </NuxtLink>

</template>

<script setup>
const getRandomInt = (min, max) => {
    return Math.floor(Math.random() * (max - min + 1)) + min
}
</script>