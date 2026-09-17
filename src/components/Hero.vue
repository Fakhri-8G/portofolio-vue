<script setup>
const socialLinks = [
  {
    name: 'GitHub',
    url: '#',
  },
  {
    name: 'Instagram',
    url: '#',
  },
  {
    name: 'Email',
    url: 'mailto:your-email@example.com',
  },
]
</script>

<template>
  <section id="home" class="hero">

    <div class="hero-background"></div>

    <div class="container hero-container">

      <!-- =====================
           HERO TEXT
      ====================== -->
      <div class="hero-content">

        <p class="hero-greeting">
          👋 Hello, I'm
        </p>

        <h1>
          Fakhri<span>.</span>
        </h1>

        <h2>
          RPL Student & Web Developer
        </h2>

        <p class="hero-description">
          Saya siswa SMK jurusan Rekayasa Perangkat Lunak
          yang sedang belajar membangun aplikasi web
          menggunakan Vue.js, Laravel, PHP, dan teknologi
          modern lainnya.
        </p>

        <!-- Buttons -->
        <div class="hero-buttons">

          <a
            href="#projects"
            class="button button-primary"
          >
            View My Projects
            <span>→</span>
          </a>

          <a
            href="#contact"
            class="button button-outline"
          >
            Contact Me
          </a>

        </div>

        <!-- Social Links -->
        <div class="social-links">

          <a
            v-for="social in socialLinks"
            :key="social.name"
            :href="social.url"
          >
            {{ social.name }}
          </a>

        </div>

      </div>


      <!-- =====================
           HERO VISUAL
      ====================== -->
      <div class="hero-visual">

        <!-- Decorative glow -->
        <div class="visual-glow"></div>

        <!-- Code Card -->
        <div class="code-card">

          <div class="code-header">

            <div class="code-dots">
              <span></span>
              <span></span>
              <span></span>
            </div>

            <span class="code-title">
              developer.js
            </span>

          </div>

          <pre><code><span class="code-keyword">const</span> developer = {
  name: <span class="code-string">"Fakhri"</span>,
  role: <span class="code-string">"RPL Student"</span>,
  skills: [
    <span class="code-string">"Vue"</span>,
    <span class="code-string">"Laravel"</span>,
    <span class="code-string">"PHP"</span>
  ]
}</code></pre>

        </div>


        <!-- Developer Card -->
        <div class="developer-card">

          <div class="developer-icon">
            &lt;/&gt;
          </div>

          <div class="developer-info">
            <strong>Fakhri</strong>
            <span>Web Developer</span>
          </div>

        </div>


        <!-- Floating tech badges -->
        <div class="tech-badge tech-vue">
          Vue
        </div>

        <div class="tech-badge tech-laravel">
          Laravel
        </div>

        <div class="tech-badge tech-php">
          PHP
        </div>

      </div>

    </div>


    <!-- Scroll indicator -->
    <a
      href="#about"
      class="scroll-indicator"
    >
      <span>↓</span>
      Scroll to explore
    </a>

  </section>
</template>