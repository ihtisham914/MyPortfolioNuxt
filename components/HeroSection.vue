<script>
import Button from "./Button.vue";
// import gsap from "gsap";

export default {
  name: "HeroSection",
  components: {
    Button,
  },
};
</script>

<template>
  <div
    class="ml-auto mr-auto pt-8rem pb-8rem pl-4rem pr-4rem md:pl-10rem md:pr-10rem lg:pl-10rem lg:pr-16rem relative bg-cyan-50 flex flex-col items-center justify-between gap-6.4rem md:flex-row lg:flex-row dark:bg-gray-700"
    id="home"
  >
    <div class="w-100% lg:w-50%">
      <p
        class="lg:mt-8.4rem text-4xl font-semibold text-center md:text-start lg:text-start"
      >
        Hi, I am Ihtisham Ul Haq
      </p>
      <h3
        class="mt-2.4rem mb-6rem lh-4rem text-center lg:text-start md:text-start"
      >
        I am a
        <span text-indigo-600 dark:text-rose-500>software Engineer</span> with
        skills in Web Development, working in different JavaScript Frameworks
        like <span text-indigo-600 dark:text-rose-500>React.js</span> and
        <span text-indigo-600 dark:text-rose-500>Vue.js</span>
      </h3>
      <div class="text-center md:text-start lg:text-start">
        <Button
          gotoid="#contact"
          title="Let's Talk"
          color="text-white"
          bgColor="bg-indigo-600"
          border="border-indigo-600"
          target="_self"
        />
        <a href="#projects"
          ><button
            class="btn text-3xl text-blue-600 bg-white ml-10rem pt-0.5rem pb-0.5rem pl-1rem pr-1rem b-rd-0.5rem border-blue-600 transition-all cursor-pointer"
            hover="text-white bg-blue-600"
          >
            My Work &darr;
          </button></a
        >
      </div>
    </div>
    <div class="flex gap-3rem flex-row lg:flex-col relative">
      <div class="flex flex-col gap-1rem absolute top-40% right-105%">
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
      <div class="hero_img lg:mt-2.4rem"></div>
    </div>
  </div>
</template>

<style scoped>
.btn:active {
  transform: scale(0.95);
}

.hero_img {
  background-image: url("../assets/images/Sham.webp");
  height: 40rem;
  width: 40rem;
  border-radius: 50%;
  background-size: cover;
}
</style>
