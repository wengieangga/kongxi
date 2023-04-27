<template>
  <div
    class="container lg:bg-transparent lg:mx-auto lg:px-20 text-red-600 py-3.5 px-6 lg:flex justify-between items-center"
  >
    <div class="flex items-center cursor-pointer">
      <span class="text-xl mr-1">
        <i class="bi bi-messenger"></i>
      </span>

      <h1 class="text-xl md:text-2xl">Kongxi</h1>
    </div>

    <span
      @click="menuOpen"
      class="absolute lg:hidden right-6 top-[12px] cursor-pointer text-4xl"
    >
      <i :class="open ? 'bi bi-x' : 'bi bi-filter-left'"></i>
    </span>

    <ul
      class="bg-black lg:bg-transparent lg:flex lg:items-center lg:px-5 px-6 lg:pb-0 pb-10 lg:static absolute lg:w-auto w-full top-14 duration-700 ease-in"
      :class="open ? 'left-0' : 'left-[-100%]'"
    >
      <li class="lg:mx-4 lg:my-2 my-6 font-medium" v-for="link in Links">
        <a
          :href="link.link"
          class="text-lg text-red-600 hover:text-white tracking-wide"
          >{{ link.name }}</a
        >
      </li>

      <Button class="lg:ml-auto w-full">Book Now</Button>
    </ul>
  </div>
</template>

<script>
import Button from "./Button.vue";
export default {
  components: {
    Button,
  },
  data() {
    const Links = [
      { name: "Home", link: "#" },
      { name: "Services", link: "#" },
      { name: "Work", link: "#" },
      { name: "Company", link: "#" },
      { name: "Blog", link: "#" },
      { name: "Contact", link: "#" },
    ];
    return {
      Links,
      open: false,
    };
  },
  methods: {
    menuOpen() {
      this.open = !this.open;
    },
  },
};
</script>
