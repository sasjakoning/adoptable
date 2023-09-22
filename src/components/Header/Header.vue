<template>
  <header>
    <Nav />
    <div>
      <h1>Adoptable</h1>
      <h2>Uw adoptie huisdier met een duurzame "paw" print.</h2>
      <a href="#">Bekijk onze dieren</a>
    </div>
    <figure class="header__media">
      <img
          class="header__media__dog-body"
          src="@/assets/dog/dog-header/dog-body.png"
          alt=""
      >
      <img
          class="header__media__dog-head"
          src="@/assets/dog/dog-header/dog-tail.png"
          alt=""
      >
    </figure>
    <button>chevron down</button>
  </header>
</template>

<script setup>
import Nav from '../Nav/Nav.vue'
</script>

<style scoped lang="scss">
@import "header";
</style>