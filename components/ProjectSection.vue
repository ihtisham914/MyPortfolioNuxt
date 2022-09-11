<script>
import Project from "./Project.vue";
export default {
  name: "ProjectSection",
  components: {
    Project,
  },
};
</script>

<template>
  <div
    class="ml-auto mr-auto pt-12rem pl-4rem pr-4rem md:pl-10rem md:pr-10rem lg:pl-10rem lg:pr-10rem"
    id="projects"
  >
    <div class="flex items-center justify-between mb-6.4rem">
      <h3 class="flex items-center gap5 text-3rem">
        <div class="i-mdi-stack-overflow text-blue-700 text-3.2rem" />
        My Projects
      </h3>
      <Button
        gotoid="https://github.com/ihtisham914"
        title="GitHub Account"
        color="text-white"
        bgColor="bg-rose-500"
        border="border-rose-500"
        target="_blank"
      />
    </div>
    <Project
      title="Chat Application => built in HTML and CSS:"
      para="Resposive Chat Application for desktop, tablet and mobile: Designed in HMTL and CSS, This Application was designed for a start up is is used as an embbed component in large application.
      This is first of my projects."
      link="https://chatresponsivedesign.netlify.app"
      code="https://github.com/ihtisham914/chatApplication.git"
      img_1="chat.webp"
    />

    <Project
      title="CharsadwaChappal => built in php:"
      para="CharsadwalChappal is an E-commerce website built for a client. It is a full stack website. I designed it and built it. you can buy Traditional Charsadwal Chappal from here as well as new trending designs."
      link="https://charsadwalchappal.000webhostapp.com/client/index.php"
      code="https://github.com/ihtisham914/charsadwalChappalphp.git"
      img_1="chappal.webp"
    />
    <Project
      title="CodingTech => built in React:"
      para="CodingTech is a simple, responsive Front-end website that is built in React. A customer can visit this site to get online services for web development. He can view profiles of the Team as well. He can contact the vendors through a form."
      link="https://codingtechreact.netlify.app"
      code="https://github.com/ihtisham914/CodingTechReact.git"
      img_1="Codingtech1.webp"
    />

    <Project
      title="Portfolio => built in Vue.js plus Nuxt.js:"
      para="My own reponsive portfolio built in vue.js and Nuxt.js. The Desing is inspired from the new trending design 'Glassmorphism'. Here I have listed all my skills. I showcased all the projects that I have been working on."
      link="https://ihtishamportfolio.netlify.app"
      code="https://github.com/ihtisham914/myportfolionuxt.git"
      img_1="portfolio.webp"
    />
  </div>
</template>
