<script setup lang="ts">
import AboutMeSection from '../components/home/AboutMeSection.vue'
import ServicesSection from '../components/home/ServicesSection.vue'
import SkillsSection from '../components/home/SkillsSection.vue'
import ToolsSection from '../components/home/ToolsSection.vue'
import ContactSection from '../components/home/ContactSection.vue'
</script>

<template>
  <HeroComponent />
  <AboutMeSection />
  <ServicesSection />
  <SkillsSection />
  <ToolsSection />
  <ContactSection />
  <PortfolioSection />
  <ReferencesSection />
</template>

<style>
.white-shape {
  svg {
    width: 100%;
  }
}

@media (max-width: 767px) {
  .white-shape {
    svg {
      width: 150%;
      height: 36px;
    }
  }
}
</style>
