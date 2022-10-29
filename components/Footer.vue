<script>
export default {
  name: "Footer",
};
</script>

<template>
  <footer
    class="mt-6.4rem text-center w-100% text-1.8rem pt-5rem pb-5rem pl-4rem pr-4rem md:pl-10rem md:pr-10rem lg:pl-10rem lg:pr-10rem bg-cyan-50 dark:text-white dark:bg-gray-800"
  >
    <div class="flex items-center justify-between pb-5rem b-b-0.2rem">
      <a class="decoration-none" href="#home">
        <img
          class="h-6.4rem mt-2rem md:h-9.4rem lg:h-9.4rem hover:op80"
          src="../assets/logo.png"
          alt=""
      /></a>

      <div class="flex flex-row gap-2rem">
        <a href="https://gitlab.com/ihtisham914" target="_blank">
          <div
            class="i-mdi-gitlab text-red-500 text-2.8rem transition-all"
            hover="text-red-400"
          />
        </a>
        <a href="https://github.com/ihtisham914" target="_blank">
          <div
            class="i-mdi-github text-gray-500 text-2.8rem transition-all"
            hover="text-gray-400"
          />
        </a>
        <a
          href="https://linkedin.com/in/ihtisham-ul-haq-998669223"
          target="_blank"
        >
          <div
            class="i-mdi-linkedin text-blue-500 text-2.8rem transition-all"
            hover="text-blue-400"
          />
        </a>
      </div>
    </div>
    <div
      class="flex items-center justify-between gap-1rem pt-2rem flex-col md:flex-row lg:flex-row"
    >
      <p>Ihtishamportfolio.com &copy; 2022</p>
      <p>
        Made with joy and hope by <span class="font-bold">Ihtisham Ul Haq</span>
      </p>
    </div>
  </footer>
</template>
