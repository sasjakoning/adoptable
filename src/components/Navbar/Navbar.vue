<template>
  <nav class="nav">
    <div class="nav__wrapper">
      <h1>Adoptable</h1>
      <button 
      @click="toggleMenu"
      aria-label="menu toggle" 
      class="nav__menu"
      ></button>
    </div>
    <ul class="nav__content">
      <li>
        <a href="#">Logo</a>
      </li>
      <li>
        <a href="#">Home</a>
      </li>
      <li>
        <a href="#">Onze dieren</a>
      </li>
      <li>
        <a href="#">Shop</a>
      </li>
      <li>
        <a href="#">Contact</a>
      </li>
      <li>
        <a href="#">cart icon</a>
      </li>
    </ul>
  </nav>
</template>

<script>

export default {
  data() {
  },

  methods: {
    toggleMenu() {
      const nav = document.querySelector('.nav__content');
      nav.classList.toggle('nav__content--active');
    },
  },
};
</script>

<style scoped lang="scss">
@import "navbar";
</style>