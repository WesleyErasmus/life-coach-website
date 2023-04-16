<template>
 <v-app>
    <v-main>
      
      <!-- Hero Component -->
      <Hero />

      <!-- Services Component -->
      <Services />

      <!-- About Component -->
      <About/>
    
    </v-main>
  </v-app>
</template>
<script>
// Home Page Components
import Hero from '../components/Hero.vue';
import Services from '../components/Services.vue';
import About from '../components/About.vue';
export default {
  components: {
    Hero,
    Services,
    About,
  }
};
</script>
