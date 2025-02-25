<template>
  <div class="container">
    <div class="floating-div">
      <div class="content">
        <h1>{{ name }}</h1>
        <h3>{{ subtitle }}</h3>
        <p>{{ description }}</p>
      </div>
    </div>
    <ParamountPlus />
    <ResumePage />
    <FSWScheduleSearch />
    <DadSite />
  </div>
</template>

<script setup>
import ParamountPlus from './ParamountPlus.vue'
import DadSite from './DadSite.vue'
import FSWScheduleSearch from './FSWScheduleSearch.vue'
import ResumePage from './ResumePage.vue'

defineProps({
  name: {
    type: String,
    default: 'David Conrad',
  },
  subtitle: {
    type: String,
    default: 'Front End Software Engineer',
  },
  description: {
    type: String,
    default: 'A website to showcase my projects and professional experience',
  },
})
</script>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  min-height: 80vh;
  padding: 2rem;
  text-align: center;
  gap: 5rem;
  margin-left: 10rem;
  margin-right: 10rem;
  margin-bottom: 5rem;
}
.floating-div {
  width: 100%;
  max-width: 800px;
  border-radius: 0;
  box-shadow: 0 2rem 4rem 0.25rem rgba(46, 43, 55, 0.4);
  background-image: linear-gradient(45deg, #726193 20%, #e37b7c 60%, #f9ae2d);
  position: relative;
  overflow: hidden;
}
.content {
  padding: 3rem;
  color: white;
}
h1 {
  font-weight: 700;
  font-size: 2.6rem;
  margin-bottom: 0.5rem;
  color: white;
  text-align: center;
}
h2 {
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
.location {
  font-size: 1.2rem;
}
.contact-info {
  font-size: 1rem;
}
.separator {
  margin: 0 0.5rem;
  color: rgba(255, 255, 255, 0.6);
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
.about-content {
  margin-top: 1rem;
}
@media (min-width: 1024px) {
  h1,
  h3,
  p {
    text-align: left;
  }
}
</style>
