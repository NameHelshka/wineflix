<template>
  <header class="hero">
    <img class="hero-image" src="/wine-hero.webp">
    <AppHeader msg="help"/>
    <div class="hero-content">
      <h2>
        <img alt="Rex Goliath" src="/rex-goliath-logo.png">
      </h2>
      <h3>His Royal Majesty is back.</h3>
      <p>
        America's most unhinged rooster is out of retirement, and this time? He's mad
        as hell.  Experience the unapologetic flavor burst of Rex Goliath.
      </p>
      <ul class="controls">
        <li>
          <button class="primary-action">
            <FontAwesomeIcon icon="play" />
            <span>Drink</span>
          </button>
        </li>
        <li>
          <button class="secondary-action">
            <FontAwesomeIcon icon="info-circle" />
            <span>More Info</span>
          </button>
        </li>
      </ul>
    </div>
  </header>
  <main>
    <section class="category">
      <h2>Drink Again</h2>
      <ul>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <span class="new-badge">New!</span>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <span class="new-badge">New!</span>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <span class="new-badge">New!</span>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
          </div>
        </li>
      </ul>
    </section>
    <section class="category">
      <h2>Keep Drinking</h2>
      <ul>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
        <li>
          <div class="wine">
            <img src="/red-wine.jpg" alt="Wine">
            <div class="amount-consumed">
              <progress min="0" max="100" value="22"></progress>
            </div>
          </div>
        </li>
      </ul>
    </section>
  </main>
</template>

<script>
import AppHeader from '@/components/AppHeader.vue';
import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  name: 'AppX',
  components: {
    FontAwesomeIcon,
    AppHeader,
  },
};
</script>

<style lang="scss">
</style>
