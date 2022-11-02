<template>
  <NavigationSection></NavigationSection>
  <HeaderSection></HeaderSection>
  <ServiceSection></ServiceSection>
  <PortfolioSection></PortfolioSection>
  <AboutSection></AboutSection>
  <TeamSection></TeamSection>
  <ClientSection></ClientSection>
  <ContactSection></ContactSection>
  <FooterSection></FooterSection>
</template>

<script>
// IMPORT EXTERNAL JS FILE
import './js/scripts.js';

// IMPORT COMPONENTS
import NavigationSection from './components/NavigationSection.vue';
import HeaderSection from './components/HeaderSection.vue';
import ServiceSection from './components/ServiceSection.vue';
import PortfolioSection from './components/PortfolioSection.vue';
import AboutSection from './components/AboutSection.vue';
import TeamSection from './components/TeamSection.vue';
import ClientSection from './components/ClientSection.vue';
import ContactSection from './components/ContactSection.vue';
import FooterSection from './components/FooterSection.vue';

export default {
  name: 'App',
  components: {
    NavigationSection,
    HeaderSection,
    ServiceSection,
    PortfolioSection,
    AboutSection,
    TeamSection,
    ClientSection,
    ContactSection,
    FooterSection,
  }
}
</script>

<style>
  @import './css/styles.css';
</style>
