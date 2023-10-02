<template>
  <section class="landing__container">
    <div class="landing__content">
      <h1>Adoptable</h1>
      <h2>Uw adoptie huisdier met een duurzame "paw" print.</h2>
    </div>
    <figure class="landing__media">
      <img
          class="landing__media__dog-body"
          src="@/assets/dog/dog-header/dog-body.png"
          alt=""
      >
      <img
          class="landing__media__dog-tail"
          src="@/assets/dog/dog-header/dog-tail.png"
          alt=""
      >
    </figure>
    <div class="landing__cta">
      <a 
      class="button"
      href="#"
      >Bekijk onze dieren</a>
      <button aria-label="down arrow" class="chevron-down"></button>
    </div>
  </section>
</template>

<script setup>

</script>

<style scoped lang="scss">
@import "landing-header.scss";
</style>