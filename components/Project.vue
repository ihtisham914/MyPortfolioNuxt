<script>
export default {
  name: "Project",
  props: {
    title: String,
    icon: String,
    iconColor: String,
    iconTitle: String,
    para: String,
    link: String,
    code: String,
    img_1: String,
  },
};
</script>

<template>
  <div
    class="flex flex-col items-center justify-between gap-3.2rem mb-6.4rem p3.2rem md:p-4.4rem lg:p-4.4rem md:flex-row lg:flex-row shadow-xl dark:bg-gray-700 b-rd-1rem"
  >
    <div class="w-100% md:w-40% lg:w-40%">
      <div class="flex items-center gap-2rem mb-2.8rem">
        <h4
          class="text-indigo-600 bg-cyan-50 dark:text-indigo-400 shadow-md p-0.3rem pr-1rem pl-1rem b-rd-0.5rem dark:text-white dark:bg-gray-600"
        >
          {{ title }}
        </h4>
        <div
          class="flex items-center justify-center bg-cyan-50 gap-1rem p-0.5rem pr-1rem pl-1rem shadow-md b-rd-0.5rem dark:bg-gray-600"
        >
          <!-- <div :class="`i-mdi-nuxt  text-green-500 text-3rem" /> -->
          <div v-if="icon == 'nuxt'" class="flex items-center mr-1rem">
            <div class="i-mdi-vuejs text-green-600 text-3rem" />
            <h5 class="text-gray-400">VueJs</h5>
          </div>
          <div :class="`i-mdi-${icon}  ${iconColor} text-3rem`" />
          <h5 class="text-gray-400">{{ iconTitle }}</h5>
        </div>
      </div>
      <p class="text-2rem mb-3.4rem">
        {{ para }}
      </p>
      <div
        class="flex gap-4.4rem items-center justify-between md:justify-initial lg:justify-initial mt-5.4rem"
      >
        <Button
          :gotoid="`${link}`"
          title="Demo"
          color="text-white"
          bgColor="bg-rose-500"
          border="border-rose-500"
          target="_blank"
        />
        <Button
          :gotoid="`${code}`"
          title="GitHub"
          color="text-rose-500"
          bgColor="bg-white"
          border="border-rose-500"
          target="_blank"
        />
      </div>
    </div>
    <div class="flex items-center justify-center h-30rem w-50rem b-rd-1rem">
      <img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        src="../static/projectImages/chat.webp"
        alt="Project images"
      />
      <img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        src="../static/projectImages/chappal.webp"
        alt="Project images"
      />
      <img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        src="../static/projectImages/Codingtech1.webp"
        alt="Project images"
      /><img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        src="../static/projectImages/portfolio.webp"
        alt="Project images"
      />
      <img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        :src="`../static/projectImages/${img_1}`"
        alt="Project images"
      />
    </div>
  </div>
</template>
