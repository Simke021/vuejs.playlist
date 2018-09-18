<template>
  <div>
    <h1>List of ninjas</h1>
      <ul>
          <li v-for="ninja in ninjas" :key = "ninja.id" >{{ ninja }}</li>
      </ul>
  </div>
</template>

<script>
export default {
  data() {
    return {
      ninjas: ["Yoshi", "Mario", "Rui"]
    };
  }
};
</script>

<style scoped>
h1 {
  color: green;
}
</style>