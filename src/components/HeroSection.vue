<template>
  <section
    class="container px-6 lg:flex lg:mx-auto lg:px-20 text-white flex items-center h-[90%] overflow-y-hidden"
  >
    <div class="lg:w-[60%]">
      <h1
        class="lg:text-5xl font-bold text-4xl leading-normal tracking-wider lg:leading-normal lg:tracking-wider"
      >
        YOUR GO-TO DIGITAL MARKETING COMPANY FOR STARTUP
      </h1>
      <p class="py-5 leading-loose">
        A top digital marketing company committed to enhancing your brand
        through branding, creative design, and multi-channel marketing
        solutions.
      </p>
      <div class="flex gap-4">
        <Button
          class="bg-transparent hover:bg-red-500 hover:border-red-500 transition-all hover:scale-[0.9]"
          >Contact Us</Button
        >
        <Button
          class="hover:border-red-500 hover:bg-transparent transition-all hover:scale-[0.9]"
          >Our Services</Button
        >
      </div>
    </div>
  </section>
</template>

<script>
import Button from "./Button.vue";
export default {
  components: { Button },
};
</script>
