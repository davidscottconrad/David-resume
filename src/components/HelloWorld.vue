<template>
  <div class="container">
    <ProjectCard
      projectName="David Conrad Portfolio"
      projectDescription="Software Developer"
      projectLink=""
      gradientStart="#726193"
      gradient-middle="#e37b7c"
      gradientEnd="#f9ae2d"
    />
    <ProjectCard
      projectName="Paramount Plus Clone"
      projectDescription="Django, Vue, and the AWS suite"
      projectLink="https://www.paramountminus.me/#/"
      gradientStart="#0460ea"
      gradientEnd="#a3bbf7"
    />
    <ProjectCard
      projectName="FSW Schedule Search"
      projectDescription="React, CodeIgniter, Docker"
      projectLink="https://www.fsw.edu/academics/schedule_search"
      gradientStart="#8b08b3"
      gradientEnd="#c17de5"
    />
    <ProjectCard
      projectName="Doctors Office Site"
      projectDescription="Next.js"
      projectLink="https://www.conradeyecenters.com/"
      gradientStart="#1e7301"
      gradientEnd="#6be7ad"
    />
    <ProjectCard
      projectName="Resume"
      projectDescription="See my resume on dropbox"
      projectLink="https://www.dropbox.com/scl/fi/tdnr1upxntd80hckpfzyz/David_Conrad_resume_02_25_25.pdf?rlkey=76bbypup8ja7l42h86rnm4ohz&st=zdkqvbpz&dl=0"
      gradientStart="#aa006c"
      gradientEnd="#ff005d"
    />
    <ProjectCard
      projectName="Github"
      projectDescription="See all my personal projects on Github"
      projectLink="https://github.com/davidscottconrad"
      gradientStart="#2b3137"
      gradientEnd="#24292e"
      style="margin-bottom: 5rem"
    />
  </div>
</template>

<script setup>
import ProjectCard from './ProjectCard.vue'

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
  text-align: center;
  gap: 3rem;
  margin-left: auto;
  margin-right: auto;
  margin-bottom: 0rem;
  margin-top: 5rem;
  width: 100%;
  max-width: 100%;
  box-sizing: border-box;
  overflow-x: hidden;
}

.floating-div {
  width: 100%;
  max-width: 800px;
  border-radius: 0;
  box-shadow: 0 1rem 2rem 0.25rem rgba(46, 43, 55, 0.4);
  background-image: linear-gradient(45deg, #726193 20%, #e37b7c 60%, #f9ae2d);
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

h2 {
  font-size: 1.2rem;
  font-weight: 700;
  margin: 1.5rem 0 0.5rem 0;
  color: white;
  text-align: center;
  letter-spacing: 0.05em;
}

h3 {
  font-size: 1.2rem;
  font-weight: 500;
  margin-bottom: 0.75rem;
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

.location {
  font-size: 1.1rem;
}

.contact-info {
  font-size: 0.9rem;
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

@media (max-width: 375px) {
  .container {
    padding: 0.5rem;
    margin-left: 0;
    margin-right: 0;
    margin-bottom: 0;
    gap: 2rem;
    max-width: 100vw;
  }

  .content {
    padding: 1.5rem;
  }

  h1 {
    font-size: 1.8rem;
  }

  h3 {
    font-size: 1rem;
  }

  p {
    font-size: 0.9rem;
  }
}

@media (min-width: 376px) and (max-width: 767px) {
  .container {
    padding: 1rem;
    margin-left: 0rem;
    margin-right: 0rem;
    margin-top: 2.5rem;
    gap: 2.5rem;

    margin-bottom: 0;
  }
}

@media (min-width: 768px) and (max-width: 1023px) {
  .container {
    margin-left: 3rem;
    margin-right: 3rem;
  }
}

html,
body {
  width: 100%;
  overflow-x: hidden;
  margin: 0;
  padding: 0;
}

@media (min-width: 1024px) {
  h1,
  h3,
  p {
    text-align: left;
  }

  .container {
    margin-left: auto;
    margin-right: auto;
    padding-left: 2rem;
    padding-right: 2rem;
    gap: 5rem;
    max-width: 1200px;
  }
}
</style>
