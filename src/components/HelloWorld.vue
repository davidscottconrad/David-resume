<script setup>
defineProps({
  msg: {
    type: String,
    required: true,
  },
})
</script>

<template>
  <div class="container">
    <div class="floating-div">
      <div class="content">
        <h1>{{ msg }}</h1>
        <h3>Welcome to the floating gradient div</h3>
        <p>
          This component features a floating animation effect with a gradient background inspired by
          the Ethereal template.
        </p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  min-height: 100vh;
  padding: 2rem;
}

.floating-div {
  width: 100%;
  max-width: 800px;
  border-radius: 0;
  box-shadow: 0 2rem 4rem 0.25rem rgba(46, 43, 55, 0.4);
  background-image: linear-gradient(45deg, #726193 20%, #e37b7c 60%, #ffe4b4);
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
  margin-bottom: 1rem;
  color: white;
  text-align: center;
}

h3 {
  font-size: 1.2rem;
  font-weight: 400;
  margin-bottom: 1.5rem;
  color: rgba(255, 255, 255, 0.9);
  text-align: center;
}

p {
  margin: 0 0 1.5rem 0;
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
