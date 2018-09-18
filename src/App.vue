<template>
  <div>
    <h1>{{ title }}</h1>
    <p>{{ greeting() }}</p>
  </div>
</template>

<script>
export default {
  data() {
    return {
      title: "My First Vue file, wooooo :)"
    };
  },
  methods: {
    greeting: function() {
      return "hey cowboy!";
    }
  }
};
</script>

<style>
</style>
