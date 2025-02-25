<template>
  <div id="container">
    <div class="floating-div">
      <a href="https://www.conradeyecenters.com" target="_blank">
        <div class="content">
          <h1>{{ name }}</h1>
          <p>{{ description }}</p>
        </div>
      </a>
    </div>
  </div>
</template>

<script setup>
defineProps({
  name: {
    type: String,
    default: 'Conrad Eye Centers',
  },
  description: {
    type: String,
    default: 'Next.js',
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
  margin-bottom: 5rem;
}

.floating-div {
  width: 100%;
  border-radius: 0;
  box-shadow: 0 2rem 4rem 0.25rem rgba(46, 43, 55, 0.4);
  background: #535353;
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
