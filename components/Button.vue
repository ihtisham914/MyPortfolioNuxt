<script>
export default {
  name: "Button",
  props: {
    gotoid: String,
    title: String,
    color: String,
    border: String,
    bgColor: String,
    target: String,
  },
};
</script>

<template>
  <a :href="`${gotoid}`" :target="`${target}`"
    ><button
      :class="`btn  ${color} ${bgColor} ${border} text-3xl pt-0.5rem pb-0.5rem pl-1rem pr-1rem lg:text-4xl lg:pt-1rem lg:pb-1rem lg:pl-2rem lg:pr-2rem md:text-3xl md:pt-0.5rem md:pb-0.5rem md:pl-1rem md:pr-1rem b-rd-0.5rem cursor-pointer transition-all`"
      hover="text-indigo-600 bg-white"
    >
      {{ title }}
    </button></a
  >
</template>

<style scoped>
.btn:active {
  transform: scale(0.95);
}
</style>
