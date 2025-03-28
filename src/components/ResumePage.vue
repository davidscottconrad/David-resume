<template>
  <div id="container">
    <div class="floating-div">
      <a :href="resumePath" download="David_Conrad_resume.pdf">
        <div class="content">
          <h1>Resume</h1>
          <!-- <p>{{ description }}</p> -->
        </div>
      </a>
    </div>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const resumePath = ref('/David_Conrad_resume_02_25_25.pdf')

defineProps({
  name: {
    type: String,
    default: 'David Conrad',
  },
  description: {
    type: String,
    default: 'Django, Vue, and the AWS suite',
  },
})
</script>

<style scoped>
#container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 20vh;
  width: 100%;
  max-width: 800px;
  margin-bottom: 4rem;
}

.floating-div {
  width: 100%;
  border-radius: 0;
  box-shadow: 0 2rem 4rem 0.25rem rgba(46, 43, 55, 0.4);
  background-image: linear-gradient(45deg, #aa006c, #ff005d);
  position: relative;
  overflow: hidden;
}

.content {
  padding: 2rem;
  color: white;
}

h1 {
  font-weight: 700;
  font-size: 2.6rem;
  margin-bottom: 0.5rem;
  color: white;
  text-align: center;
}

h3 {
  font-size: 1.4rem;
  font-weight: 700;
  margin: 1.5rem 0 0.5rem 0;
  color: white;
  text-align: center;
  letter-spacing: 0.05em;
}

p {
  margin: 0 0 0.5rem 0;
  font-size: 1.1rem;
  line-height: 1.6;
  color: rgba(255, 255, 255, 0.9);
  text-align: center;
}

@media (min-width: 1024px) {
  h1,
  h3,
  p {
    text-align: left;
  }
}
</style>
