<script setup>
import Header from "@/components/Header.vue";
import Footer from "@/components/Footer.vue";
import WhoAmI from "@/components/WhoAmI.vue";
import AboutMe from "@/components/AboutMe.vue";
import MyJourney from "@/components/MyJourney.vue";
import MyArts from "@/components/MyArts.vue";
import Tools from "@/components/Tools.vue";

import { onMounted } from "vue";
import { initFlowbite } from "flowbite";
import ApproachMe from "./components/ApproachMe.vue";

// initialize components based on data attribute selectors
onMounted(() => {
  initFlowbite();
});
</script>

<template>
  <header class="fixed top-0 left-0 right-0 z-50">
    <Header />
  </header>

  <main class="max-w-screen-lg px-4 mx-auto">
    <!-- who am i -->
    <WhoAmI />

    <!-- about me -->
     <AboutMe />

    <!-- my journey -->
     <MyJourney />

    <!-- my arts -->
     <MyArts />

    <!-- tools and skills -->
    <Tools /> 

    <!-- approach me -->
     <ApproachMe /> 
    
  </main>

  <footer>
    <Footer />
  </footer>
</template>

<script>
export default {
  
};
</script>
