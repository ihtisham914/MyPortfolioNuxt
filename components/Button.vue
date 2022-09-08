<script>
export default {
  name: "Button",
  props: {
    gottid: String,
    title: String,
  },
};
</script>

<template>
  <a href="#contact"
    ><button class="btn">
      {{ title }}
    </button></a
  >
</template>

<style scoped>
.btn {
  font-family: "Nunito", sans-serif;
  font-size: 1.8rem;
  color: #fff;
  padding: 0.5rem 1rem;
  border-radius: 0.5rem;
  border: none;
  cursor: pointer;

  background: linear-gradient(to bottom right, #e35af3, #9e00f9);
  transition: all 0.3s;
}

.btn:hover {
  background: linear-gradient(to bottom right, #9e00f9, #e35af3);
}

.btn:active {
  transform: scale(0.95);
}

@media only screen and (max-width: 430px) {
  .btn {
    font-size: 1.6rem;
    padding: 0.35rem 0.7rem;
  }
}
</style>
