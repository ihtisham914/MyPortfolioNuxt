<template>
  <header>
    <div>
      <a class="logo" href="#home"> Ihtisham Ul Haq</a>
    </div>
    <ul class="links">
      <li><a href="#home">Home</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
    <div v-show="!show" class="link_icon_open">
      <div class="i-mdi-menu text-blue-700" text-15 @click="showMenu" />
    </div>
    <div v-show="show" class="link_icon">
      <div class="i-mdi-close text-blue-700" text-15 @click="showMenu" />
    </div>
    <ul v-show="show" class="menu_links">
      <li><a href="#home">Home</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </header>
</template>

<script>
export default {
  name: "Header",
  data() {
    return {
      show: false,
    };
  },
  methods: {
    showMenu() {
      this.show = !this.show;
    },
  },
};
</script>

<style scoped>
header {
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 2rem 8rem;
  width: 100%;
  height: 7.4rem;

  background-color: rgba(255, 255, 255, 0.2);
  border-radius: 0 0 1.6rem 1.6rem;
  box-shadow: rgba(0, 0, 0, 0.5);
  backdrop-filter: blur(5rem);

  position: sticky;
  z-index: 2;
  top: 0;
}

.logo {
  color: #fff;
  font-size: 2.8rem;
  font-weight: 700;
  text-decoration: none;
}

ion-icon {
  display: none;
  visibility: hidden;
}

.link_icon {
  display: inline-block;
  visibility: visible;
}

.link_icon_open,
.menu_links,
.link_icon {
  display: none;
  visibility: hidden;
}

.links {
  display: flex;
  visibility: visible;
  align-items: center;
  justify-content: space-between;
  gap: 4rem;
  list-style: none;
}

.menu_links {
  display: flex;
  visibility: visible;
  flex-direction: column;
  align-items: flex-start;
  gap: 3rem;
  border-radius: 1.6rem;
  background-color: #b24fecc5;
  backdrop-filter: blur(5rem);
  list-style: none;
  width: 30%;
  padding: 2rem 4rem !important;

  position: absolute;
  z-index: 2;
  top: 0;
  right: 0;
  transform: translate(100%, 26%);
}

/* ul.menu_links li {
  margin-left: 4rem;
} */

ul li a {
  text-decoration: none;
  color: #fff;
  font-weight: 200;
  transition: all 0.3s;
  border-bottom: 2px solid #ffffff1a;
  padding-bottom: 0.3rem;
  letter-spacing: 0.1rem;
}

li {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 7rem;
}

ul li a:hover,
ul li a:active,
ul a a:visited {
  border-bottom: 2px solid blue;
  font-size: 2.6rem;
  /* color: blueviolet; */
}

/* media queries */
@media only screen and (max-width: 930px) {
  ion-icon {
    display: inline-block;
    visibility: visible;
  }
  .links {
    display: none;
    visibility: hidden;
  }

  .menu_links {
    display: flex;
    visibility: visible;
  }

  .link_icon {
    display: inline-block;
    visibility: visible;
  }

  .menu_links {
    transform: translate(0%, 26%);
  }

  .link_icon_open {
    display: inline-block;
    visibility: visible;
  }
}

@media only screen and (max-width: 530px) {
  .menu_links {
    width: 50%;
  }
}

@media only screen and (max-width: 430px) {
  .logo {
    font-size: 2.4rem;
  }
}
</style>
