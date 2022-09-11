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
    class="flex flex-col items-center justify-between gap-3.2rem mb-6.4rem p3.2rem md:p-4.4rem lg:p-4.4rem md:flex-row lg:flex-row shadow-xl dark:bg-gray-700 b-rd-1rem"
  >
    <div class="w-100% md:w-40% lg:w-40%">
      <h4 class="mb-2.8rem text-indigo-600 dark:text-indigo-400">
        {{ title }}
      </h4>
      <p class="text-2rem mb-3.4rem">
        {{ para }}
      </p>
      <div
        class="flex gap-4.4rem items-center justify-between md:justify-initial lg:justify-initial"
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
          color="text-white"
          bgColor="bg-rose-500"
          border="border-rose-500"
          target="_blank"
        />
      </div>
    </div>
    <div class="flex items-center justify-center h-30rem w-50rem b-rd-1rem">
      <img
        class="h-100% w-40rem ml-0 md:w-45rem lg:w-45rem b-rd-1rem"
        :src="`static/projectImages/${img_1}`"
        alt="Project images"
      />
    </div>
  </div>
</template>
