<script setup>
const skills = [
  {
    name: 'Vue.js',
    category: 'Frontend',
    description: 'Membangun interface web yang interaktif dengan Vue.',
    level: 'Learning',
    icon: 'V',
  },
  {
    name: 'Laravel',
    category: 'Backend',
    description: 'Membangun backend dan REST API menggunakan Laravel.',
    level: 'Learning',
    icon: 'L',
  },
  {
    name: 'PHP',
    category: 'Backend',
    description: 'Bahasa pemrograman yang saya gunakan untuk backend.',
    level: 'Learning',
    icon: 'PHP',
  },
  {
    name: 'JavaScript',
    category: 'Programming',
    description: 'Digunakan untuk membuat logic dan interaksi web.',
    level: 'Learning',
    icon: 'JS',
  },
  {
    name: 'HTML & CSS',
    category: 'Frontend',
    description: 'Membangun struktur dan tampilan website.',
    level: 'Learning',
    icon: '</>',
  },
  {
    name: 'Git & GitHub',
    category: 'Tools',
    description: 'Version control dan kolaborasi dalam project.',
    level: 'Learning',
    icon: 'Git',
  },
]
</script>

<template>
  <section id="skills" class="skills-section">

    <div class="container">

      <!-- Section Heading -->
      <div class="section-heading skills-heading">

        <span class="section-label">
          MY SKILLS
        </span>

        <h2>
          Technologies I
          <span>work with.</span>
        </h2>

        <p>
          Beberapa teknologi yang sedang saya pelajari
          dan gunakan dalam project.
        </p>

      </div>


      <!-- Skills Grid -->
      <div class="skills-grid">

        <article
          v-for="skill in skills"
          :key="skill.name"
          class="skill-card"
        >

          <!-- Icon -->
          <div class="skill-icon">
            {{ skill.icon }}
          </div>


          <!-- Content -->
          <div class="skill-content">

            <div class="skill-title-row">

              <h3>
                {{ skill.name }}
              </h3>

              <span class="skill-level">
                {{ skill.level }}
              </span>

            </div>

            <span class="skill-category">
              {{ skill.category }}
            </span>

            <p>
              {{ skill.description }}
            </p>

          </div>


          <!-- Arrow -->
          <span class="skill-arrow">
            →
          </span>

        </article>

      </div>


      <!-- Bottom Note -->
      <div class="skills-note">

        <span>💡</span>

        <p>
          Saya masih terus belajar dan menambah teknologi
          baru melalui project dan pengalaman praktik.
        </p>

      </div>

    </div>

  </section>
</template>