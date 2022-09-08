<script>
import Button from "./Button.vue";
// import gsap from "gsap";

export default {
  name: "HeroSection",
  components: {
    Button,
  },
};
</script>

<template>
  <div class="hero_container glass" id="home">
    <div class="hero_section flex">
      <div class="intro">
        <h3>Hi, I am Ihtisham Ul Haq</h3>
        <p class="intro_para">
          I am a software Engineer with skills in Web Development, working in
          different JavaScript Frameworks like React.js and Vue.js
        </p>
        <div class="btns">
          <Button gotoid="contact" title="Let's Talk" class="btn_one" />
          <a href="#projects" class="btn_two"
            ><button class="btn">My Work &darr;</button></a
          >
        </div>
      </div>
      <div class="img_container">
        <div class="icons_links">
          <a href="https://gitlab.com/ihtisham914" target="_blank">
            <div class="i-mdi-gitlab text-white-700" text-10 />
          </a>
          <a href="https://github.com/ihtisham914" target="_blank">
            <div class="i-mdi-github text-white-700" text-10 />
          </a>
          <a
            href="https://linkedin.com/in/ihtisham-ul-haq-998669223"
            target="_blank"
          >
            <div class="i-mdi-linkedin text-white-700" text-10 />
          </a>
        </div>

        <div class="hero_img"></div>
      </div>
    </div>
  </div>
</template>

<style scoped>
h3 {
  margin-top: 2.8rem;
}
.btns {
  display: flex;
  align-items: center;
  gap: 7rem;
}

.btn {
  font-family: "Nunito", sans-serif;
  font-size: 1.8rem;
  font-weight: 500;
  color: #6b4bd6;
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  border: 1px solid #6b4bd6;
  cursor: pointer;
  transition: all 0.3s;
}

.btn:hover {
  background-color: #6b4bd6;
  color: #fff;
}

.btn:active {
  transform: scale(0.95);
}

.glass {
  background-color: rgba(255, 255, 255, 0.2);
  border-radius: 1.6rem;
  box-shadow: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(3rem);
}
.hero_section {
  /* gap: 27rem; */
  height: 70vh;
}

.intro {
  width: 50%;
}

.intro_para {
  font-weight: 600;
  font-size: 2.4rem;
  margin: 2.4rem 0 6rem 0;
}
.hero_img {
  background-image: url("../assets/images/Sham.webp");
  height: 40rem;
  width: 40rem;
  border-radius: 50%;
  background-size: cover;

  /* outline: 0.5rem solid #c86ee3; */
  box-shadow: 0 0 18px 18px #c86ee390;
}
.hero_container {
  position: relative;
  margin: 4.4rem 10rem 6.4rem 10rem;
  padding: 2.4rem;
}

.img_container {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 3rem;
}

.icons_links {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 1rem;
  transition: all 0.5s;
}

.icons_links a {
  transition: all 0.3s;
  color: #fff;
}

.icons_links a:nth-child(1):hover {
  color: red;
}

.icons_links a:nth-child(2):hover {
  color: grey;
}

.icons_links a:nth-child(3):hover {
  color: #6b4bd6;
}

/* Media Queries */
@media only screen and (max-width: 830px) {
  .hero_section {
    height: 80%;
  }

  .intro,
  .intro_para {
    text-align: center;
  }

  .btns {
    justify-content: space-around;
  }
}

@media only screen and (max-width: 600px) {
  .hero_section {
    height: 90%;
  }

  .intro {
    width: 64%;
  }

  .img_container {
    flex-direction: column;
  }
  .icons_links {
    flex-direction: row;
    gap: 3rem;
  }
}

@media only screen and (max-width: 430px) {
  .hero_container {
    margin: 2.4rem 2rem 6.4rem 2rem;
  }
}

@media only screen and (max-width: 430px) {
  .btn {
    font-size: 1.4rem;
    padding: 0.3rem 0.6rem;
  }
}
</style>
