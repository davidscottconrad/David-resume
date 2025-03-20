<template>
  <div class="project-container">
    <div class="project-card" :style="cardStyle">
      <a :href="projectLink" target="_blank">
        <div class="content">
          <h1>{{ projectName }}</h1>
          <p>{{ projectDescription }}</p>
        </div>
      </a>
    </div>
  </div>
</template>

<script setup>
import { computed } from 'vue'

const props = defineProps({
  projectName: {
    type: String,
    required: true,
  },
  projectDescription: {
    type: String,
    required: true,
  },
  projectLink: {
    type: String,
    required: true,
  },
  gradientStart: {
    type: String,
    default: '#726193',
  },
  gradientMiddle: {
    type: String,
    default: '',
  },
  gradientEnd: {
    type: String,
    default: '#f9ae2d',
  },
  gradientDirection: {
    type: String,
    default: '45deg',
  },
})

const cardStyle = computed(() => {
  if (props.gradientMiddle) {
    return {
      backgroundImage: `linear-gradient(${props.gradientDirection}, ${props.gradientStart} 20%, ${props.gradientMiddle} 60%, ${props.gradientEnd})`,
    }
  }

  return {
    backgroundImage: `linear-gradient(${props.gradientDirection}, ${props.gradientStart}, ${props.gradientEnd})`,
  }
})
</script>

<style scoped>
.project-container {
  display: flex;
  justify-content: center;
  align-items: center;
  width: 100%;
  max-width: 800px;
  margin: 0 auto;
}

.project-card {
  width: 100%;
  max-width: 800px;
  border-radius: 0;
  box-shadow: 0 1rem 2rem 0.25rem rgba(46, 43, 55, 0.4);
  position: relative;
  overflow: hidden;
  box-sizing: border-box;
}

.content {
  padding: 2rem;
  color: white;
}

h1 {
  font-weight: 700;
  font-size: 2rem;
  margin-bottom: 0.5rem;
  color: white;
  text-align: center;
}

p {
  margin: 0 0 0.5rem 0;
  font-size: 1rem;
  line-height: 1.5;
  color: rgba(255, 255, 255, 0.9);
  text-align: center;
  word-wrap: break-word;
}

a {
  color: white;
  text-decoration: none;
  transition: color 0.2s;
}

a:hover {
  color: #ffe4b4;
  text-decoration: underline;
}

/* Media Queries for Responsiveness */
/* Small phones */
@media (max-width: 375px) {
  .content {
    padding: 1.5rem;
  }
  h1 {
    font-size: 1.8rem;
  }
  p {
    font-size: 0.9rem;
  }
}

/* Desktop view */
@media (min-width: 1024px) {
  h1,
  p {
    text-align: left;
  }
}
</style>
