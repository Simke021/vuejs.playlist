<template>
    <div>
        <app-header></app-header>
        <app-main v-bind:ninjas="ninjas"></app-main>
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
    return {
      ninjas: [
        { name: "Ryu", speciality: "Vue Components", show: false },
        { name: "Crystal", speciality: "HTML Wizardry", show: false },
        { name: "Hitoshi", speciality: "Click Events", show: false },
        { name: "Tango", speciality: "Conditionals", show: false },
        { name: "Kami", speciality: "Webpack", show: false },
        { name: "Yoshi", speciality: "Data Diggin", show: false }
      ]
    };
  }
};
</script>

<style>
body {
  margin: 0;
  font-family: "Nunito SemiBold";
  background-color: #efefef;
}
</style>