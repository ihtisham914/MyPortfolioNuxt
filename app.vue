<template>
  <div id="app">
    <!-- <h1 text-20 op30>hello world</h1> -->
    <!-- <NuxtWelcome /> -->
    <Header />
    <HeroSection />
    <SkillSection />
    <ProjectSection />
    <ContactSection />
    <Footer />
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

  font-size: 2.4rem;
  font-weight: 400;
  color: #fff;
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

#app {
  /* max-width: 1300px; */
  height: 100%;
  margin: 0 auto;

  font-weight: normal;
  background-image: url(assets/images/background.webp);
  background-size: cover;
}

h3 {
  letter-spacing: 0.2rem;
  font-size: 2.4rem;
  font-weight: 400;
}

h3.heading {
  font-size: 2.4rem;
  font-weight: 700;
}

h4 {
  font-size: 2.2rem;
}
.container {
  margin: 4.4rem 10rem 4rem 10rem;
  padding: 9.4rem 4rem 4rem 4rem;
}

.container:last-child {
  margin-bottom: 0;
}
.glass {
  background-color: rgba(255, 255, 255, 0.1);
  border-radius: 1.6rem;
  box-shadow: rgba(0, 0, 0, 0.2);
  backdrop-filter: blur(3rem);
}

.flex {
  display: flex;
  align-items: center;
  justify-content: space-between;
}
.grid-cols-3 {
  display: grid;
  grid-template-columns: repeat(3, 1fr);
}
.grid-cols-4 {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
}

/* Media queries */
@media only screen and (max-width: 1200px) {
  /*Tablets [601px -> 1200px]*/
  html {
    font-size: 55%;
  }
}

@media only screen and (max-width: 900px) {
  .grid-cols-3 {
    grid-template-columns: repeat(2, 1fr);
  }
  html {
    font-size: 50%;
  }
}

@media only screen and (max-width: 830px) {
  .flex {
    flex-direction: column;
    gap: 5rem;
  }
}

@media only screen and (max-width: 600px) {
  /*Big smartphones [426px -> 600px]*/
  .flex {
    flex-direction: column;
    gap: 5rem;
  }
}
@media only screen and (max-width: 430px) {
  /*Small smartphones [325px -> 425px]*/
  .grid-cols-3 {
    grid-template-columns: repeat(1, 1fr);
  }

  .container {
    margin: 2.4rem 2rem 6.4rem 2rem;
  }
}

@media only screen and (max-width: 400px) {
  html {
    font-size: 45%;
  }
}
</style>
