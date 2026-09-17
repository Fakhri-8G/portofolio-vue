<script setup>
  import Navbar from './components/Navbar.vue'

  const name = 'Fakhri'
  const role = 'Web Developer & RPL Student'
</script>

<template>
  <Navbar />

  <main id="home">
    <h1>Hi, I'm {{ name }}</h1>
    <p>{{ role }}</p>
  </main>
</template>