<script>
import Skill from "./Skill.vue";
import Button from "./Button.vue";

export default {
  name: "SkillSection",
  components: {
    Skill,
    Button,
  },
};
</script>

<template>
  <div
    class="ml-auto mr-auto pt-12rem pl-4rem pr-4rem md:pl-10rem md:pr-10rem lg:pl-10rem lg:pr-10rem"
    id="skills"
  >
    <h3 class="text-3.2rem mb-6.8rem flex items-center justify-initial gap-5">
      <div class="i-mdi-account-cog text-indigo-600 text-4rem" />
      Skilled In Technologies
    </h3>
    <div class="grid grid-cols-1 md:grid-cols-3 lg:grid-cols-3 gap-3.2rem">
      <Skill
        icon="language-html5"
        iconColor="html"
        heading="HTMl and CSS"
        para="Want to build a responsive website in HTML and CSS, here I am. I can create bueatiful
      design based on your content with custom CSS."
        borderColor="htmlShadow"
      />
      <Skill
        icon="language-javascript"
        iconColor="javascript"
        heading="JavaScript"
        para="Want to build a dynamic website, here I am. I can create a fully flegde front-end dynamic website in JavaScript."
        borderColor="javascriptShadow"
      />
      <Skill
        icon="language-php"
        heading="PHP"
        iconColor="php"
        para="Want to build a full-stack website in php, here I am. I can create a full-stack dynamic website in PHP."
        borderColor="phpShadow"
      />
      <Skill
        icon="react"
        heading="React.js"
        iconColor="react"
        para="Want to build front-end for your website in react, here I am. I can create a fully dynamic front-end in react."
        borderColor="reactShadow"
      />

      <Skill
        icon="vuejs"
        heading="Vue.js"
        iconColor="vue"
        para="Want to build front-end for your website in vue, here I am. I can create a fully dynamic front-end in vue."
        borderColor="vueShadow"
      />
      <div class="talk">
        <div
          class="i-mdi-account-question-outline text-white-700"
          text-20
          color-rose
        />
        <h3 class="heading_sure">Not sure yet!</h3>
        <p>If you are not sure about your Project, let's talk about it ...</p>
        <Button
          gotoid="#contact"
          title="Let's Talk"
          color="text-white"
          bgColor="bg-indigo-600"
          border="border-indigo-600"
        />
      </div>
    </div>
  </div>
</template>

<style scoped>
.talk {
  display: flex;
  align-items: center;
  justify-content: center;
  flex-direction: column;
  gap: 2rem;
  padding: 2rem;
}

.heading_sure {
  font-weight: 600;
  margin-bottom: 0;
  text-align: center;
}
p {
  font-size: 1.6rem;
  text-align: center;
}

h3 {
  margin-bottom: 4.8rem;
}
</style>
