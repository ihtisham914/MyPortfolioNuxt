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
  <div class="container glass" id="skills">
    <h3 class="heading text-50px" flex align-center gap-5>
      <div class="i-mdi-user text-blue-700" text-15 />
      Skilled In Technologies
    </h3>
    <div class="grid-cols-3">
      <Skill
        icon="language-html5"
        iconColor="html"
        heading="HTMl and CSS"
        para="Want to build a responsive website in HTML and CSS, here I am. I can create bueatiful
      design based on your content with custom CSS."
        color="#c092f9"
      />
      <Skill
        icon="language-javascript"
        iconColor="javascript"
        heading="JavaScript"
        para="Want to build a dynamic website, here I am. I can create a fully flegde front-end dynamic website in JavaScript."
        color="#EB99AF"
      />
      <Skill
        icon="language-php"
        heading="PHP"
        iconColor="php"
        para="Want to build a full-stack website in php, here I am. I can create a full-stack dynamic website in PHP."
        color="#C84ED4"
      />
      <Skill
        icon="react"
        heading="React.js"
        iconColor="react"
        para="Want to build front-end for your website in react, here I am. I can create a fully dynamic front-end in react."
        color="#C84ED4"
      />

      <Skill
        icon="vuejs"
        heading="Vue.js"
        iconColor="vue"
        para="Want to build front-end for your website in vue, here I am. I can create a fully dynamic front-end in vue."
        color="#c092f9"
      />
      <div class="talk">
        <div
          class="i-mdi-account-question-outline text-white-700"
          text-20
          color-rose
        />
        <h3 class="heading_sure">Not sure yet!</h3>
        <p>If you are not sure about your Project, let's talk about it ...</p>
        <Button title="Let's Talk" color="#fff" bgcolor="#3C2DE8BD" />
      </div>
    </div>
  </div>
</template>

<style scoped>
.grid-cols-3 {
  gap: 2rem;
}

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

.before_enter {
  opacity: 0;
  transform: translateY(200px);
  transition: all 2s ease-out;
}

.enter {
  opacity: 1;
  transform: translateY(0px);
}
</style>
