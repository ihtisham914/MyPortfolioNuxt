<script>
export default {
  name: "ContactSection",
};
</script>

<template>
  <div
    id="contact"
    class="mb-4.6rem ml-auto mr-auto pt-8.6rem pl-2rem pr-2rem md:pl-10rem md:pr-10rem lg:pl-10rem lg:pr-10rem"
  >
    <h3 class="mb-2.4rem text-center">Let's build something amazing for you</h3>
    <div
      class="flex items-center justify-between lg:justify-center md:gap-2.4rem lg:gap-4.4rem flex-col md:flex-row lg:flex-row"
    >
      <div class="w-70% md:w-59% lg:w-40% p-2rem">
        <form
          class="flex flex-col justify-center gap-3rem"
          action="https://formspree.io/f/moqbvdvr"
          method="post"
        >
          <input
            class="pt-2 pb-2 pl-4 pr-4 b-rd-3rem text-1.8rem outline-none max-w-40rem h-5rem text-indigo-600 bg-white b-indigo-600"
            type="text"
            required
            placeholder="Your Name"
            name="name"
          />
          <input
            class="pt-2 pb-2 pl-4 pr-4 b-rd-3rem text-1.8rem outline-none max-w-40rem h-5rem text-indigo-600 bg-white b-indigo-600"
            name="email"
            type="email"
            required
            placeholder="What's your Email"
          />
          <textarea
            class="pt-2 pb-2 pl-4 pr-4 b-rd-3rem text-1.8rem outline-none max-w-40rem h-12rem text-indigo-600 bg-white b-indigo-600"
            name="description"
            id="problem"
            placeholder="Just say it :)"
          ></textarea>
          <button
            class="max-w-40rem p-1.2rem mt-3rem text-white uppercase text-2.2rem b-rd-3rem border-none cursor-pointer transition-all"
            focus="outline-none"
            type="submit"
          >
            Let's do it
          </button>
        </form>
      </div>
      <div
        class="contact_image mt-6.4rem h-45rem w-95% md:w-69% lg:w-45% b-rd-1rem"
      ></div>
    </div>
  </div>
</template>

<style scoped>
.contact_image {
  background: linear-gradient(
      to right bottom,
      rgba(72, 0, 253, 0.12),
      rgba(255, 0, 225, 0.12)
    ),
    url("../assets/images/contactimage.webp");
  background-size: cover;
  background-position: center;
}

button {
  background: linear-gradient(to bottom right, #e35af3, #9e00f9);
}

button:hover {
  background: linear-gradient(to bottom right, #9e00f9, #e35af3);
}
button:active {
  transform: scale(0.95);
}
</style>
