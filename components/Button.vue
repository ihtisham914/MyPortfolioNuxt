<script>
export default {
  name: "Button",
  props: {
    gottid: String,
    title: String,
  },
};
</script>

<template>
  <a href="#contact"
    ><button
      gotoid="gotoid"
      class="btn text-3xl text-white bg-indigo-600 pt-0.5rem pb-0.5rem pl-1rem pr-1rem b-rd-0.5rem b-rd-0.5rem border-indigo-600 cursor-pointer transition-all"
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
