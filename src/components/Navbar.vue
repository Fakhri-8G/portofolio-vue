<script setup>
import { ref } from 'vue'

const isMenuOpen = ref(false)

const navItems = [
  { name: 'Home', href: '#home' },
  { name: 'About', href: '#about' },
  { name: 'Skills', href: '#skills' },
  { name: 'Projects', href: '#projects' },
  { name: 'Journey', href: '#journey' },
  { name: 'Contact', href: '#contact' },
]

const closeMenu = () => {
  isMenuOpen.value = false
}
</script>

<template>
  <header class="navbar">

    <div class="navbar-container">

      <!-- Logo -->
      <a
        href="#home"
        class="logo"
        @click="closeMenu"
      >
        Fakh<span>ri</span>
      </a>

      <!-- Desktop Navigation -->
      <nav class="nav-links">
        <a
          v-for="item in navItems"
          :key="item.name"
          :href="item.href"
        >
          {{ item.name }}
        </a>
      </nav>

      <!-- Theme Button -->
      <button
        class="theme-button"
        aria-label="Toggle theme"
      >
        ☼
      </button>

      <!-- Mobile Menu Button -->
      <button
        class="menu-button"
        aria-label="Toggle navigation"
        @click="isMenuOpen = !isMenuOpen"
      >
        <span v-if="!isMenuOpen">☰</span>
        <span v-else>✕</span>
      </button>

    </div>

    <!-- Mobile Navigation -->
    <nav
      v-if="isMenuOpen"
      class="mobile-nav"
    >
      <a
        v-for="item in navItems"
        :key="item.name"
        :href="item.href"
        @click="closeMenu"
      >
        {{ item.name }}
      </a>
    </nav>

  </header>
</template>