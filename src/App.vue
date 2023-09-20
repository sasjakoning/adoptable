<template>
  <header>
    <nav>
      <ul>
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
    <div>
      <h1>Adoptable</h1>
      <h2>Uw adoptie huisdier met een duurzame "paw" print.</h2>
      <a href="#">Bekijk onze dieren</a>
    </div>
    <figure>
      <img src="" alt="">
    </figure>
    <button>chevron down</button>
  </header>
  <main>
    <section>
      <h2>Ons adoptie proces in vier stappen</h2>
      <ol>
        <li>
          <figure>
            <img src="" alt="">
          </figure>
          <h3>Bekijk onze dieren ter adoptie</h3>
        </li>
        <li>
          <figure>
            <img src="" alt="">
          </figure>
          <h3>Plan een ontmoetings afspraak</h3>
        </li>
        <li>
          <figure>
            <img src="" alt="">
          </figure>
          <h3>Kies een essentials pakket</h3>
        </li>
        <li>
          <figure>
            <img src="" alt="">
          </figure>
          <h3>Adopteer!</h3>
        </li>
      </ol>
      <span></span>
    </section>
    <section>
      <h2>Onze dieren in het zonnetje</h2>
      <ul>
        <li>
          <figure>
            <img src="https://source.unsplash.com/random/296*352/?pet" alt="">
            <figcaption>
              <h3>Bonnie</h3>
              <div>
                <p>Boxer</p>
                <p>2 jaar</p>
              </div>
            </figcaption>
          </figure>
        </li>
      </ul>
    </section>
  </main>
</template>


<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style>
