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
        color="text-rose-500"
        bgColor="bg-white"
        border="border-rose-500"
        target="_blank"
      />
    </div>
    <Project
      title="Chat Application"
      iconTitle="HTML and CSS"
      icon="language-html5"
      iconColor="html"
      para="Resposive Chat Application for desktop, tablet and mobile: Designed in HMTL and CSS, This Application was designed for a start up is is used as an embbed component in large application.
      This is first of my projects."
      link="https://chatresponsivedesign.netlify.app"
      code="https://github.com/ihtisham914/chatApplication.git"
      img_1="chat.webp"
      direction="normal"
    />

    <Project
      title="CharsadwaChappal"
      iconTitle="PHP"
      icon="language-php"
      iconColor="php"
      para="CharsadwalChappal is an E-commerce website built for a client. It is a full stack website. I designed it and built it. you can buy Traditional Charsadwal Chappal from here as well as new trending designs."
      link="https://charsadwalchappal.000webhostapp.com/client/index.php"
      code="https://github.com/ihtisham914/charsadwalChappalphp.git"
      img_1="chappal.webp"
      direction="reverse"
    />
    <Project
      title="CodingTech"
      iconTitle="Reactjs"
      icon="react"
      iconColor="react"
      para="CodingTech is a simple, responsive Front-end website that is built in React. A customer can visit this site to get online services for web development. He can view profiles of the Team as well. He can contact the vendors through a form."
      link="https://codingtechreact.netlify.app"
      code="https://github.com/ihtisham914/CodingTechReact.git"
      img_1="Codingtech1.webp"
      direction="normal"
    />

    <Project
      title="Portfolio"
      iconTitle="Nuxtjs"
      icon="nuxt"
      iconColor="nuxt"
      para="My own reponsive portfolio built in vue.js and Nuxt.js. The Desing is inspired from the new trending design 'Glassmorphism'. Here I have listed all my skills. I showcased all the projects that I have been working on."
      link="https://ihtishamportfolio.netlify.app"
      code="https://github.com/ihtisham914/myportfolionuxt.git"
      img_1="portfolio.webp"
      direction="reverse"
    />

    <Project
      title="DevHub"
      iconTitle="Reactjs"
      icon="react"
      iconColor="react"
      para="DevHub is a simple, responsive Front-end website that is built in React with tailwind. Here you can find software developers and see their description. You can add developers to help it grow."
      link="https://developershubreact.netlify.app"
      code="https://github.com/ihtisham914/DevelopersHub.git"
      img_1="devhub.png"
      direction="normal"
    />
  </div>
</template>
