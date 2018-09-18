<template>
    <div>
        <app-header></app-header>
        <app-main></app-main>
        <app-footer></app-footer>
    </div>
</template>

<script>
// Imports
import Header from "./components/Header.vue";
import Main from "./components/Main.vue";
import Footer from "./components/Footer.vue";
export default {
  components: {
    "app-header": Header,
    "app-main": Main,
    "app-footer": Footer
  },
  data() {
    return {};
  }
};
</script>

<style>
body {
  margin: 0;
  font-family: "Nunito SemiBold";
}
</style>