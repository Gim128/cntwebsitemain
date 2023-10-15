<template>
  <v-main>
    <navigation-menu />
    <hero-component />
    <!-- <counter-component /> -->
    <feature-component />
    <CAT_Component />
    <select-componnet />
    <!-- <footer-component /> -->
    <FooterView />
  </v-main>
</template>

<script>
// import FooterComponent from './components/FooterComponent.vue';
import HeroComponent from "./components/HeroComponent.vue";
import FeatureComponent from "./components/FeatureComponent.vue";
// import NavbarComponent from './components/NavbarComponent.vue';
// import CounterComponent from './components/CounterComponent.vue';
import CAT_Component from "./components/CAT_Component.vue";
import SelectComponnet from "./components/SelectComponnet.vue";
import NavigationMenu from "./components/NavigationMenu.vue";
import FooterView from "./components/FooterView.vue";
// import NavbarView from './components/NavbarView.vue';

export default {
  name: "App",

  components: {
    // NavbarComponent,
    HeroComponent,
    FeatureComponent,
    // FooterComponent,
    // CounterComponent,
    CAT_Component,
    SelectComponnet,
    NavigationMenu,
    FooterView,
  },

  data: () => {
    //
  },
};
</script>
