<script>
export default {
  name: 'ContactSection',
}
</script>

<template>
  <div id="contact" class="contact_container container glass">
    <h3 class="heading">Let's build something amazing for you</h3>
    <div class="flex">
      <div class="contact_form">
        <form action="https://formspree.io/f/moqbvdvr" method="post">
          <input
            class="input"
            type="text"
            required
            placeholder="Your Name"
            name="name"
          />
          <input
            class="input"
            name="email"
            type="email"
            required
            placeholder="What's your Email"
          />
          <textarea
            class="input"
            name="description"
            id="problem"
            placeholder="Just say it :)"
          ></textarea>
          <button type="submit">Let's do it</button>
        </form>
      </div>
      <div class="contact_image"></div>
    </div>
  </div>
</template>

<style scoped>
h3 {
  text-align: center;
  margin-bottom: 3.4rem;
}

.contact_image {
  height: 45rem;
  width: 45%;
  border-radius: 1rem;
  box-shadow: 0 0 18px 18px #c86ee390;

  background: linear-gradient(
      to right bottom,
      rgba(72, 0, 253, 0.12),
      rgba(255, 0, 225, 0.12)
    ),
    url('../assets/images/contactimage.webp');
  background-size: cover;
  background-position: center;
}

.contact_form {
  width: 40%;
  padding: 2rem;
}

form {
  display: flex;
  flex-direction: column;
  justify-content: center;
  gap: 3rem;
}

.input {
  padding: 0.5rem 2rem;
  border-radius: 3rem;
  font-size: 1.8rem;
  outline: none;
  border: 2px solid #0356f190;
  max-width: 40rem;
  height: 5rem;
  color: rgb(248, 41, 223);
  background-color: rgb(237, 235, 235);
}

.input:focus {
  background-color: #fff;
}

.input:nth-child(3) {
  height: 12rem;
}

button {
  max-width: 40rem;
  padding: 1.2rem;
  margin-top: 3rem;
  color: #fff;
  text-transform: uppercase;
  font-size: 2.2rem;
  letter-spacing: 3px;
  border-radius: 3rem;
  border: none;
  background: linear-gradient(to bottom right, #e35af3, #9e00f9);
  cursor: pointer;
  transition: all 0.3s;
}

button:hover {
  background: linear-gradient(to bottom right, #9e00f9, #e35af3);
}
button:active {
  transform: scale(0.95);
}

button:focus {
  outline: none;
}

/* media queries */
@media only screen and (max-width: 830px) {
  .contact_form {
    width: 59%;
  }

  .contact_image {
    width: 69%;
  }
}

@media only screen and (max-width: 600px) {
  .contact_form {
    width: 92%;
  }

  .contact_image {
    width: 95%;
  }
}
</style>
