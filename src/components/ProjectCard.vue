<script setup>
defineProps({
  project: {
    type: Object,
    required: true,
  },
})
</script>

<template>
  <article class="project-card">

    <!-- Project Image -->
    <div class="project-image">
      <div class="project-image-content">
        <span class="project-number">
          {{ project.number }}
        </span>

        <span class="project-type">
          {{ project.type }}
        </span>
      </div>
    </div>


    <!-- Project Content -->
    <div class="project-content">

      <div class="project-meta">
        <span>{{ project.year }}</span>
        <span>•</span>
        <span>{{ project.role }}</span>
      </div>


      <h3>
        {{ project.title }}
      </h3>


      <p>
        {{ project.description }}
      </p>


      <!-- Technologies -->
      <div class="project-tech">

        <span
          v-for="tech in project.technologies"
          :key="tech"
        >
          {{ tech }}
        </span>

      </div>


      <!-- Link -->
      <a
        v-if="project.link"
        :href="project.link"
        target="_blank"
        rel="noopener noreferrer"
        class="project-link"
      >
        View Project
        <span>→</span>
      </a>

    </div>

  </article>
</template>