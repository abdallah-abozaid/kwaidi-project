<template>
  <FstNavbar />
  <SecNavbar />
  <router-view />
  <app-footer />
  <div class="contact">
    <a href="/">
      <img src="./assets/contact.png" alt="contact" />
    </a>
  </div>
</template>
<script>
import AppFooter from "./components/AppFooter/AppFooter.vue";
import FstNavbar from "./components/AppHeader/FstNavbar.vue";
import SecNavbar from "./components/AppHeader/SecNavbar.vue";
export default {
  name: "App",
  components: { FstNavbar, SecNavbar, AppFooter },
};
</script>
<style lang="scss">
@font-face {
  font-family: "DIN Next LT Arabic bold";
  src: url(../public/fonts/BOLD.otf);
}
@font-face {
  font-family: "DIN Next LT Arabic mediam";
  src: url(../public/fonts/MEDIUM.otf);
}
@font-face {
  font-family: "DIN Next LT Arabic light";
  src: url(../public/fonts/LIGHT.otf);
}
@keyframes moving {
  0% {
    transform: translateY(0);
  }
  100% {
    transform: translateY(-10px);
  }
}
.contact {
  position: fixed;
  right: 10px;
  bottom: 0px;
  transition: all 0.3s linear;
  img {
    width: 90px;
    animation: moving 1s linear infinite alternate;
  }
  &:hover {
    transform: scale(1.1);
  }
}
#app {
  direction: rtl;
  font-family: "DIN Next LT Arabic mediam", sans-serif;
  font-style: normal;
  overflow: hidden;
}
a {
  text-decoration: none !important;
  color: #000;
}
nav {
  padding: 30px;

  a {
    font-weight: bold;
    color: #2c3e50;

    &.router-link-exact-active {
      color: #42b983;
    }
  }
}
h4.title {
  position: relative;
  padding-right: 10px;
  padding-top: 5px;
  color: rgba(95, 95, 95, 1);
  font-family: "DIN Next LT Arabic mediam", sans-serif;
}
h4.title::after {
  content: "";
  background-color: #3ac2cb;
  width: 3px;
  height: 100%;
  position: absolute;
  top: -10%;
  right: 0;
}
</style>
