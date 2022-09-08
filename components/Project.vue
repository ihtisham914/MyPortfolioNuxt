<script>
export default {
  name: "Project",
  props: {
    title: String,
    para: String,
    link: String,
    code: String,
    img_1: String,
  },
};
</script>

<template>
  <div class="project glass flex">
    <div class="project_left">
      <h4 class="project_heading">
        {{ title }}
      </h4>
      <p class="project_description">
        {{ para }}
      </p>
      <span style="margin-right: 1rem; font-size: 2.2rem">Link:</span
      ><a :href="`${link}`" target="_blank">Visite site</a><br />
      <span style="margin-right: 1rem; font-size: 2.2rem">Code: </span
      ><a :href="`${code}`" target="_blank">GitHub</a>
    </div>
    <div class="img_container">
      <img
        class="img"
        :src="`../assets/images/${img_1}`"
        alt="Project images"
      />
    </div>
  </div>
</template>

<style scoped>
.project {
  margin-bottom: 6.4rem;
  padding: 3rem;
}
.project_left {
  width: 40%;
}

.project_heading {
  margin-bottom: 2.8rem;
}

.project_description {
  font-size: 2rem;
  margin-bottom: 3.4rem;
}

a {
  color: #fff;
  font-size: 1.8rem;
  transition: all 0.3s;
}

a:hover {
  text-decoration: none;
}

.img_container {
  display: flex;
  align-items: center;
  justify-content: center;
  height: 30rem;
  width: 50rem;
  border-radius: 1rem;
}

.img {
  height: 100%;
  width: 45rem;
  border-radius: 1rem;
}

.before_enter {
  opacity: 0;
  transform: translateX(1000px);
  transition: all 2s ease-out;
}

.enter {
  opacity: 1;
  transform: translateX(0px);
}

/* media queries */

@media only screen and (max-width: 830px) {
  .project_left {
    width: 95%;
  }
}

@media only screen and (max-width: 430px) {
  .project_left {
    width: 95%;
  }

  .img {
    width: 40rem;
    margin-left: none;
  }
}
</style>
