<template>
  <header
    class="flex flex-row justify-between pt-8 pb-8 pr-16 pl-16 md:pr-45 md:pl-40 lg:pr-45 lg:pl-40 top-0 z-2 sticky bg-gray-50/10 backdrop-blur dark:bg-gray-900/50 light:text-white h-7.4rem w-100% relative"
  >
    <div>
      <a class="text-black text-5xl font-semibold decoration-none" href="#home">
        Ihtisham Ul Haq</a
      >
    </div>
    <ul class="hidden md:hidden lg:flex justify-between gap-2rem list-none">
      <li>
        <a
          href="#home"
          class="text-black p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >Home</a
        >
      </li>
      <li>
        <a
          href="#skills"
          class="text-black p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >Skills</a
        >
      </li>
      <li>
        <a
          href="#about"
          class="text-black p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >About</a
        >
      </li>
      <li>
        <a
          href="#projects"
          class="text-black p-1rem transition-all decoration-none"
          hover="text-indigo-600"
          >Projects</a
        >
      </li>
      <li>
        <a
          href="#contact"
          class="text-black p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >Contact</a
        >
      </li>
      <li><div class="i-mdi-white-balance-sunny text-black text-13" /></li>
      <!-- <li><div class="i-mdi-moon-waning-crescent text-white text-13" /></li> -->
    </ul>
    <div v-show="!show" class="block md:block lg:hidden">
      <div class="i-mdi-menu text-indigo-600" text-15 @click="showMenu" />
    </div>
    <div v-show="show" class="block md:block lg:hidden">
      <div class="i-mdi-close text-indigo-600" text-15 @click="showMenu" />
    </div>
    <ul
      v-show="show"
      class="flex flex-col align-start gap-2rem list-none p-4rem h-90vh w-30rem absolute top-29 right-15 md:right-40 md:flex lg:hidden bg-cyan-50 dark:bg-gray-900/50"
    >
      <li>
        <a
          href="#home"
          class="text-black p-1rem transition-all decoration-none"
          hover="font-semibold"
          >Home</a
        >
      </li>
      <li>
        <a
          href="#skills"
          class="text-black p-1rem transition-all decoration-none"
          hover="font-semibold"
          >Skills</a
        >
      </li>
      <li>
        <a
          href="#about"
          class="text-black p-1rem transition-all decoration-none"
          hover="font-semibold"
          >About</a
        >
      </li>
      <li>
        <a
          href="#projects"
          class="text-black p-1rem transition-all decoration-none"
          hover="font-semibold"
          >Projects</a
        >
      </li>
      <li>
        <a
          href="#contact"
          class="text-black p-1rem transition-all decoration-none"
          hover="font-semibold"
          >Contact</a
        >
      </li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      show: false,
    };
  },
  methods: {
    showMenu() {
      this.show = !this.show;
      console.log("click");
    },
  },
};
</script>

<style scoped>
/* li {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 7rem;
} */
</style>
