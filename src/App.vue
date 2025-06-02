<template>
  <div class="font-sans bg-gray-900 text-white">
    <HeroSection />
    <About />
    <Projects />
    <Skills />
    <Contact />
    <Footer />
  </div>
</template>

<script>
import HeroSection from './components/HeroSection.vue'
import About from './components/About.vue'
import Projects from './components/Projects.vue'
import Skills from './components/Skills.vue'
import Contact from './components/Contact.vue'
import Footer from './components/Footer.vue'

export default {
  components: { HeroSection, About, Projects, Skills, Contact, Footer }
}
</script>
