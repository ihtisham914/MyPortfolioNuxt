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
      :class="`btn text-3xl ${color} ${bgColor} ${border} pt-0.5rem pb-0.5rem pl-1rem pr-1rem b-rd-0.5rem cursor-pointer transition-all`"
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
