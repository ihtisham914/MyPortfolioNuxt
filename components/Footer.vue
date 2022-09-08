<script>
export default {
  name: "Footer",
};
</script>

<template>
  <footer class="glass">
    <p>Ihtishamportfolio.com &copy; 2022</p>
    <p>Designed and Developed by Ihtisham Ul Haq</p>
  </footer>
</template>

<style scoped>
footer {
  margin-top: 6.4rem;
  text-align: center;
  width: 100%;
  font-size: 1.8rem;
  padding: 1rem;
}

.glass {
  border-radius: 1rem 1rem 0 0;
}

p {
  letter-spacing: 0.2rem;
  margin: 1rem;
}

p:last-child {
  margin-bottom: 0.5rem;
}
</style>
