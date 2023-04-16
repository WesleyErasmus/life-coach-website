<template>
 <v-app>
    <v-main>
      
      <!-- Hero Component -->
      <Hero />

      <!-- Services Component -->
      <Services />
    
    </v-main>
  </v-app>
</template>
<script>
// Home Page Components
import Hero from '../components/Hero.vue';
import Services from '../components/Services.vue';
export default {
  components: {
    Hero,
    Services,
  }
};
</script>
