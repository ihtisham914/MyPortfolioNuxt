<script>
export default {
  name: "Skill",

  props: {
    icon: String,
    iconColor: String,
    heading: String,
    para: String,
    color: String,
  },
};
</script>

<template>
  <div class="skill" :style="{ background: color }">
    <div class="icons">
      <div :class="`i-mdi-${icon} text-white-700 ${iconColor}`" text-30 />
    </div>
    <h3 class="heading">{{ heading }}</h3>
    <p>{{ para }}</p>
  </div>
</template>

<style scoped>
.skill {
  display: flex;
  flex-direction: column;
  gap: 1.6rem;
  /* background-color: #adf992; */
  padding: 2rem;
  border-radius: 1rem;
  box-shadow: rgba(0, 0, 0, 0.5);
  transition: all 0.3s;
  cursor: pointer;
}

.skill:hover {
  transform: translateY(-0.5rem);
}

.icons {
  display: flex;
  gap: 1rem;
}

p {
  font-size: 2rem;
}

h3 {
  margin-top: 2rem;
}

/* classes for color of icons */
.html {
  color: orangered;
}

.javascript {
  color: rgb(233, 233, 21);
}

.php {
  color: blue;
}

.react {
  color: skyblue;
}

.vue {
  color: #42ad74;
}
</style>
