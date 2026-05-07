<script setup>
import Navbar from './components/Navbar.vue'
import HeroSection from './components/HeroSection.vue'
import About from './components/About.vue'
import Projects from './components/Project.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'
import ClickSpark from './components/ClickSpark.vue'
</script>

<template>
    <ClickSpark
    spark-color="#ff6b6b"
    :spark-size="12"
    :spark-radius="25"
    :spark-count="12"
    :duration="600"
    easing="ease-out"
    :extra-scale="1.2"
  >
  <div class="grid-bg min-h-screen">
  <Navbar />
  <HeroSection />
  <About />
  <Projects />
  <Contact />
  <Footer />
  </div>
    </ClickSpark>
</template>
