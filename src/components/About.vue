<script setup>
const stats = [
  {
    number: '01+',
    label: 'Years Learning',
  },
  {
    number: '05+',
    label: 'Projects',
  },
  {
    number: '05+',
    label: 'Technologies',
  },
]
</script>

<template>
  <section id="about" class="about-section">

    <div class="container">

      <!-- Section Heading -->
      <div class="section-heading">
        <span class="section-label">ABOUT ME</span>

        <h2>
          A little bit about
          <span>me.</span>
        </h2>

        <p>
          Mengenal saya lebih jauh dan perjalanan saya
          dalam dunia pengembangan software.
        </p>
      </div>


      <!-- About Content -->
      <div class="about-grid">

        <!-- About Text -->
        <div class="about-content">

          <p class="about-intro">
            Halo, saya Fakhri 👋
          </p>

          <p>
            Saya adalah siswa SMK jurusan Rekayasa Perangkat
            Lunak yang memiliki ketertarikan pada dunia
            pemrograman dan pengembangan aplikasi.
          </p>

          <p>
            Saat ini saya sedang mempelajari bagaimana
            membangun aplikasi web dari sisi frontend
            maupun backend menggunakan berbagai teknologi
            modern.
          </p>

          <p>
            Saya senang belajar dengan membuat project nyata,
            karena dari setiap project saya bisa memahami
            bagaimana sebuah aplikasi dirancang, dibuat,
            dan dikembangkan.
          </p>

          <!-- Stats -->
          <div class="about-stats">

            <div
              v-for="stat in stats"
              :key="stat.label"
              class="stat-item"
            >
              <strong>{{ stat.number }}</strong>
              <span>{{ stat.label }}</span>
            </div>

          </div>

        </div>


        <!-- About Card -->
        <div class="about-card-wrapper">

          <div class="about-card">

            <div class="about-card-top">
              <div class="about-avatar">
                F
              </div>

              <div>
                <strong>Fakhri</strong>
                <span>RPL Student</span>
              </div>
            </div>


            <div class="about-card-divider"></div>


            <div class="about-info">

              <div class="info-row">
                <span class="info-label">Focus</span>
                <span class="info-value">
                  Web Development
                </span>
              </div>

              <div class="info-row">
                <span class="info-label">Learning</span>
                <span class="info-value">
                  Vue & Laravel
                </span>
              </div>

              <div class="info-row">
                <span class="info-label">Education</span>
                <span class="info-value">
                  SMK — RPL
                </span>
              </div>

              <div class="info-row">
                <span class="info-label">Goal</span>
                <span class="info-value">
                  Informatics
                </span>
              </div>

            </div>


            <div class="about-card-footer">
              <span class="status-dot"></span>
              Currently learning & building
            </div>

          </div>

        </div>

      </div>

    </div>

  </section>
</template>