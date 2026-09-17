<script setup>
import ProjectCard from './ProjectCard.vue'

const projects = [
  {
    number: '01',
    title: 'FixIT',
    type: 'School Project',
    year: '2026',
    role: 'Backend Developer',
    description:
      'Sistem laporan kerusakan fasilitas sekolah yang membantu siswa dan pihak sekolah dalam melaporkan serta mengelola kerusakan.',
    technologies: [
      'Laravel',
      'Vue.js',
      'MySQL',
    ],
    link: '#',
  },

  {
    number: '02',
    title: 'Toko Seragam',
    type: 'PKL Project',
    year: '2026',
    role: 'Web Developer',
    description:
      'Website e-commerce untuk penjualan seragam sekolah dan custom class shirt dengan fitur pemesanan dan pembayaran.',
    technologies: [
      'Laravel',
      'Livewire',
      'Tailwind CSS',
    ],
    link: '#',
  },

  {
    number: '03',
    title: 'Insta Space',
    type: 'PKL Project',
    year: '2026',
    role: 'Web Developer',
    description:
      'Sistem reservasi ruang untuk membantu pengelolaan property, unit, booking, review, dan informasi ruang.',
    technologies: [
      'Laravel',
      'Livewire',
      'Folio',
    ],
    link: '#',
  },

  {
    number: '04',
    title: 'Portfolio Website',
    type: 'Personal Project',
    year: '2026',
    role: 'Frontend Developer',
    description:
      'Website portfolio pribadi untuk menampilkan profil, skill, project, perjalanan belajar, dan kontak.',
    technologies: [
      'Vue.js',
      'JavaScript',
      'CSS',
    ],
    link: '#',
  },
]
</script>

<template>
  <section id="projects" class="projects-section">

    <div class="container">

      <!-- Section Heading -->
      <div class="section-heading projects-heading">

        <span class="section-label">
          MY PROJECTS
        </span>

        <h2>
          Things I've
          <span>built.</span>
        </h2>

        <p>
          Beberapa project yang pernah saya kerjakan
          selama belajar dan mengembangkan kemampuan
          di dunia software development.
        </p>

      </div>


      <!-- Projects -->
      <div class="projects-grid">

        <ProjectCard
          v-for="project in projects"
          :key="project.number"
          :project="project"
        />

      </div>


      <!-- Bottom -->
      <div class="projects-bottom">

        <p>
          More projects coming soon...
        </p>

      </div>

    </div>

  </section>
</template>