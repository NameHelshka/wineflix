<template>
  <header class="hero">
    <img class="hero-image" src="/wine-hero.webp">
    <!--<AppHeader msg="help"/>-->
    <nav class="navigation">

      <section class="primary-navigation">
        <h1>WineFlix</h1>
        <ul class="navigation-links">
          <li
            v-for="navigationLink in navigationLinks"
            :key="navigationLink.label"
            :class="navigationLink.isActive"
          >
            <NavigationLink
              :url="navigationLink.url"
              :label="navigationLink.label"
            />
          </li>
        </ul>
      </section>

      <section class="secondary-navigation">
        <userAvatar :username="computedUsername"/>
      </section>

    </nav>
    <div class="hero-content">
      <h2>
        <img alt="Rex Goliath" src="/rex-goliath-logo.png">
      </h2>
      <h3>His Royal Majesty is back.</h3>
      <p>
        America's most unhinged rooster is out of retirement, and this time? He's mad as hell.  Experience the unapologetic flavor burst of Rex Goliath.
      </p>
      <ul class="controls">
        <li>
          <LinkButton :icon="btnDrink.icon" :classname="btnDrink.class" :text="btnDrink.text"/>
        </li>
        <li>
          <LinkButton :icon="btnMoreInfo.icon" :classname="btnMoreInfo.class" :text="btnMoreInfo.text"/>
        </li>
      </ul>
    </div>
  </header>
  <main>

    <DrinkAgainSection header_text="Drink Again" :data_list="drinkAgainList"/>
    <KeepDrinkingSection header_text="Keep Drinking" :data_list="keepDrinkingList"/>

  </main>
</template>

<script>

import NavigationLink from '@/components/NavigationLink.vue';
import DrinkAgainSection from '@/components/DrinkAgainSection';
import KeepDrinkingSection from "@/components/KeepDrinkingSection";
import UserAvatar from "@/components/UserAvatar";
import LinkButton from "@/components/LinkButton";

import { FontAwesomeIcon } from '@fortawesome/vue-fontawesome';

export default {
  name: 'App',
  components: {
    DrinkAgainSection,
    KeepDrinkingSection,
    NavigationLink,
    UserAvatar,
    LinkButton,
  },
  computed: {
    computedUsername() {
        return "Helshka";
    },
    btnDrink() {
      return {icon: 'play', class: 'primary-action', text: 'Drink'}
    },
    btnMoreInfo() {
      return {icon: 'info-circle', class: 'secondary-action', text: 'More Info'}
    },
    navigationLinks() {
      return [{
        label: "Home",
        url: "#",
        isActive: true,
      },{
        label: "Whites",
        url:"#",
        isActive: false,
      }, {
        label: "Reds",
        url: "#",
        isActive: false,
      }, {
        label: "Blends",
        url:"#",
        isActive: false,
        }];
    },
    drinkAgainList() {
      return [{
        id: 1,
        isNew: true,
      },{
        id: 2,
        isNew: false,
      }, {
        id: 3,
        isNew: true,
      }, {
        id: 4,
        isNew: true,
      }, {
        id: 5,
        isNew: false,
      }];
    },
    keepDrinkingList() {
      return [{
        id: 1,
        progress: 20,
      },{
        id: 2,
        progress: 36,
      }, {
        id: 3,
        progress: 66,
      }, {
        id: 4,
        progress: 10,
      }];
    },

  }
};
</script>

<style lang="scss">
</style>
