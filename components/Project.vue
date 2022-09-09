<script>
export default {
  name: "Project",
  props: {
    title: String,
    para: String,
    link: String,
    code: String,
    img_1: String,
  },
};
</script>

<template>
  <div
    class="flex flex-col items-center justify-between gap-3.2rem mb-6.4rem p3.2rem md:p-4.4rem lg:p-4.4rem md:flex-row lg:flex-row shadow-lg dark:bg-gray-700 b-rd-1rem"
  >
    <div class="w-100% md:w-40% lg:w-40%">
      <h4 class="mb-2.8rem text-indigo-600 dark:text-indigo-400">
        {{ title }}
      </h4>
      <p class="text-2rem mb-3.4rem">
        {{ para }}
      </p>
      <span class="mr-1rem text-2.2rem">Link:</span
      ><a
        class="text-black text-1.8rem transition-all dark:text-white"
        hover="decoration-none text-indigo-600"
        :href="`${link}`"
        target="_blank"
        >Visit site</a
      ><br />
      <span class="mr-1rem text-2.2rem">Code: </span
      ><a
        class="text-black text-1.8rem transition-all dark:text-white"
        hover="decoration-none text-indigo-600"
        :href="`${code}`"
        target="_blank"
        >GitHub</a
      >
    </div>
    <div class="flex items-center justify-center h-30rem w-50rem b-rd-1rem">
      <img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        :src="`${img_1}`"
        alt="Project images"
      />
    </div>
  </div>
</template>
