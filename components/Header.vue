<template>
  <header
    class="flex flex-row justify-between pt-8 pb-8 pr-16 pl-16 md:pr-45 md:pl-40 lg:pr-45 lg:pl-40 top-0 z-2 sticky bg-gray-50/10 backdrop-blur dark:bg-gray-900/50 light:text-white h-7.4rem w-100% relative"
  >
    <div>
      <a
        class="text-black dark:text-white text-5xl font-semibold decoration-none"
        href="#home"
      >
        Ihtisham Ul Haq</a
      >
    </div>
    <ul class="hidden md:hidden lg:flex justify-between gap-2rem list-none">
      <li>
        <a
          href="#home"
          class="text-black dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >Home</a
        >
      </li>
      <li>
        <a
          href="#skills"
          class="text-black dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >Skills</a
        >
      </li>
      <li>
        <a
          href="#about"
          class="text-black dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >About</a
        >
      </li>
      <li>
        <a
          href="#projects"
          class="text-black dark:text-white p-1rem transition-all decoration-none"
          hover="text-indigo-600"
          >Projects</a
        >
      </li>
      <li>
        <a
          href="#contact"
          class="text-black dark:text-white p-1rem transition-all decoration-none"
          hover=" text-indigo-600"
          >Contact</a
        >
      </li>
      <li>
        <div
          :class="`dark:i-mdi-white-balance-sunny i-mdi-moon-waning-crescent text-black text-13 dark:text-white`"
          @click="toggleDark"
        />
      </li>
    </ul>
    <div
      :class="`dark:i-mdi-white-balance-sunny i-mdi-moon-waning-crescent text-black text-13 dark:text-white lg:hidden`"
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
