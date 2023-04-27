<template>
  <div
    class="bg-black h-screen bg-[url('assets/hero-section.jpg')] bg-no-repeat bg-center"
  >
    <Navbar />
    <HeroSection />
  </div>
</template>

<script>
import Navbar from "./components/Navbar.vue";
import HeroSection from "./components/HeroSection.vue";

export default {
  name: "App",
  components: { Navbar, HeroSection },
};
</script>
