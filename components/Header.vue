<template>
  <header
    class="flex flex-row items-center justify-between h-7.4rem pt-8 pb-8 pr-16 pl-16 md:pr-45 md:pl-40 lg:pr-45 lg:pl-40 top-0 z-2 sticky bg-gray-50/10 backdrop-blur dark:bg-gray-900/50 light:text-white w-100% relative"
  >
    <a class="decoration-none" href="#home">
      <img class="mt-2rem h-5.4rem hover:op80" src="../assets/logo.png" alt=""
    /></a>

    <ul class="hidden md:hidden lg:flex justify-between gap-2rem list-none">
      <li>
        <a
          href="#home"
          class="text-gray-600 dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600 dark:text-rose-500"
          >Home</a
        >
      </li>
      <li>
        <a
          href="#skills"
          class="text-gray-600 dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600 dark:text-rose-500"
          >Skills</a
        >
      </li>
      <li>
        <a
          href="#about"
          class="text-gray-600 dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600 dark:text-rose-500"
          >About</a
        >
      </li>
      <li>
        <a
          href="#projects"
          class="text-gray-600 dark:text-white p-1rem transition-all decoration-none"
          hover="text-indigo-600 dark:text-rose-500"
          >Projects</a
        >
      </li>
      <li>
        <a
          href="#contact"
          class="text-gray-600 dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600 dark:text-rose-500"
          >Contact</a
        >
      </li>
      <li>
        <div
          class="i-mdi-white-balance-sunny dark:i-mdi-moon-waning-crescent text-gray-600 text-13 dark:text-white cursor-pointer"
          hover="text-black dark:text-gray-300"
          @click="toggleDark"
        />
      </li>
    </ul>
    <div
      class="i-mdi-white-balance-sunny dark:i-mdi-moon-waning-crescent text-black text-13 dark:text-white lg:hidden cursor-pointer"
      @click="toggleDark"
    />
  </header>
</template>
<script setup lang="ts">
const color = useColorMode();

function toggleDark() {
  color.preference = color.value === "dark" ? "light" : "dark";
  console.log("clicked");
}
</script>

<style scoped>
/* li {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 7rem;
} */
</style>
