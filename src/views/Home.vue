<template>
 <v-app>
    <v-main>    
      <!-- Hero Component -->
      <Hero @click="scrollToAnchor" />

      <div id="anchor"></div>
      <!-- Services Component -->
      <Services />

      <!-- About Component -->
      <About/>

      <!-- Testimonials Component -->
      <Testimonials/>

      <!-- Let's get to Work Component -->
      <GetInTouch/>

      <!-- Contact footer Component -->
      <Contact/>
    
    </v-main>
  </v-app>
</template>
<script>
// Home Page Components
import Hero from '../components/Hero.vue';
import Services from '../components/Services.vue';
import About from '../components/About.vue';
import Testimonials from '../components/Testimonials.vue';
import GetInTouch from '../components/GetInTouch.vue';
import Contact from '../components/Contact.vue';
export default {
  components: {
    Hero,
    Services,
    About,
    Testimonials,
    GetInTouch,
    Contact,
  },
    methods: {
    scrollToAnchor() {
      const element = document.getElementById("anchor");
      element.scrollIntoView({ behavior: "smooth" });
    },
  },
};
</script>
