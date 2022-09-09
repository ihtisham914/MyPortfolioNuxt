<template>
  <div
    id="app"
    class="text-2.4rem dark:text-white dark:bg-gray-700 text-black bg-white relative"
  >
    <Header />
    <HeroSection />
    <SkillSection />
    <About />
    <ProjectSection />
    <ContactSection />
    <Footer />
    <NavBar />
  </div>
</template>

<style>
* {
  padding: 0;
  margin: 0;
  box-sizing: border-box;
}

html {
  font-size: 62.5%;
  scroll-behavior: smooth;
}

body {
  font-family: "Nunito", sans-serif;
}

body::-webkit-scrollbar {
  width: 12px;
}
body::-webkit-scrollbar-track {
  background: rgb(255, 255, 255, 0.5);
}
body::-webkit-scrollbar-thumb {
  background-color: rgb(250, 156, 172);
  border-radius: 20px;
  border: 3px solid rgb(255, 255, 255, 0.5);
}

/* Media queries */
@media only screen and (max-width: 1200px) {
  html {
    font-size: 55%;
  }
}

@media only screen and (max-width: 900px) {
  html {
    font-size: 50%;
  }
}

@media only screen and (max-width: 400px) {
  html {
    font-size: 45%;
  }
}
</style>
