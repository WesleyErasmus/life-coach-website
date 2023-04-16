<template>
 <v-app>
    <v-main>
      <div>Make a my experience section</div>
      
      <!-- Hero Component -->
      <Hero />

      <!-- Services Component -->
      <Services />

      <!-- About Component -->
      <About/>

      <!-- Testimonials Component -->
      <Testimonials/>
    
    </v-main>
  </v-app>
</template>
<script>
// Home Page Components
import Hero from '../components/Hero.vue';
import Services from '../components/Services.vue';
import About from '../components/About.vue';
import Testimonials from '../components/Testimonials.vue';
export default {
  components: {
    Hero,
    Services,
    About,
    Testimonials,
  }
};
</script>
