<script>
export default {
  name: "Skill",

  props: {
    icon: String,
    iconColor: String,
    heading: String,
    para: String,
    borderColor: String,
  },
};
</script>

<template>
  <div
    :class="`skill flex flex-col bg-cyan-50 gap-1.6rem p-3rem b-rd-1rem transition-all cursor-pointer dark:text-white dark:bg-gray-800 ${borderColor}`"
    data-aos="fade-up"
  >
    <!-- <div :class="`i-mdi-language-html5  ${iconColor}`"  text-30 />
    <div
      :class="`i-mdi-language-javascript  ${iconColor}`"
      text-30
    />0
    <div :class="`i-mdi-language-php  ${iconColor}`" text-30 />
    <div :class="`i-mdi-react  ${iconColor}`"  text-30 />
    <div :class="`i-mdi-vuejs  ${iconColor}`" text-30 /> -->
    <div :class="`i-mdi-${icon}  ${iconColor} text-35`" />
    <h3 class="mt-2rem text-2.4rem text-indigo-600 dark:text-indigo-400">
      {{ heading }}
    </h3>
    <p>{{ para }}</p>
  </div>
</template>

<style>
.skill:hover {
  transform: translateY(-0.5rem);
}

/* classes for color of icons */
.html {
  color: orangered;
}

.htmlShadow {
  box-shadow: 1px 6px 5px 0px orangered;
}

.javascript {
  color: #e9e915;
}

.javascriptShadow {
  box-shadow: 0px 3px 5px 1px #e9e915;
}

.php {
  color: blue;
}

.phpShadow {
  box-shadow: 0px 3px 5px 1px blue;
}

.react {
  color: skyblue;
}

.reactShadow {
  box-shadow: 0px 3px 5px 1px skyblue;
}

.vue {
  color: #42ad74;
}

.vueShadow {
  box-shadow: 0px 3px 5px 1px #42ad74;
}

.nuxt {
  color: #4ade80;
}
</style>
