<template>
  <nav
    :ref="nr"
    class="navbar navbar-expand-lg change"
    :class="theme === 'light' ? 'light' : ''"
  >
    <div class="container">
      <NuxtLink to="/" class="logo">
          <img
            ref="lr"
            src="/img/logo-dark.png"
            v-if="theme === 'light'"
            alt="logo"
          />
          <img
            ref="lr"
            src="/img/logo-light.png"
            v-else-if="theme === 'themeD'"
            alt="logo"
          />
          <img ref="lr" src="/img/logo-light.png" v-else alt="logo" />
      </NuxtLink>

      <button
        class="navbar-toggler"
        type="button"
        @click="handleMobileDropdown"
        data-toggle="collapse"
        data-target="#navbarSupportedContent"
        aria-controls="navbarSupportedContent"
        aria-expanded="false"
        aria-label="Toggle navigation"
      >
        <span class="icon-bar">
          <i class="fas fa-bars"></i>
        </span>
      </button>

      <div class="collapse navbar-collapse" id="navbarSupportedContent">
        <ul class="navbar-nav ml-auto">
          <li class="nav-item">
            <a href="#anasayfa" class="nav-link"> Anasayfa</a>
          </li>
          <li class="nav-item">
            <a href="#ozelliklerim" class="nav-link"> Özelliklerim</a>
          </li>
          <li class="nav-item">
            <a href="#portfolıo" class="nav-link"> Portfolıo</a>
          </li>
          <li class="nav-item">
            <a href="#yetenekler" class="nav-link"> Yetenekler</a>
          </li>
          <li class="nav-item">
            <a href="#bizeulasin" class="nav-link"> Bize Ulaşın</a>
          </li>
        </ul>
      </div>
    </div>
  </nav>
</template>

<script>
import getSiblings from "../../common/getSiblings";
export default {
  props: ["lr", "theme", "nr"],
  methods: {
    handleDropdown: (e) => {
      getSiblings(e.target.parentElement)
        .filter((item) => item.classList.contains("show"))
        .map((item) => {
          item.classList.remove("show");
          if (item.childNodes[0]) {
            item.childNodes[0].setAttribute("aria-expanded", false);
          }
          if (item.childNodes[2]) {
            item.childNodes[2].classList.remove("show");
          }
        });
      e.target.setAttribute("aria-expanded", true);
      if (e.target.parentElement) {
        e.target.parentElement.classList.toggle("show");
        let dropdownMenu = e.target.parentElement.childNodes[2];
        if (dropdownMenu) {
          dropdownMenu.classList.toggle("show");
        }
      }
    },
    handleMobileDropdown: (e) => {
      document
        .getElementById("navbarSupportedContent")
        .classList.toggle("show-with-trans");
    },
  },
};
</script>

<style scoped>
</style>
