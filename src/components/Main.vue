<template>
    <div id="ninjas">
      <ul>
          <li v-for="ninja in ninjas" :key = "ninja.id" v-on:click="ninja.show = !ninja.show">
              <h2>{{ ninja.name }}</h2>
              <h3 v-show="ninja.show">{{ ninja.speciality }}</h3>
          </li>
      </ul>
    </div>
</template>
<script>
export default {
  props: {
    ninjas: {
      type: Array,
      required: true
    }
  },
  data() {
    return {};
  }
};
</script>
<style scoped>
#ninjas {
  width: 100%;
  max-width: 1200px;
  margin: 40px auto;
  padding: 0 20px;
  box-sizing: border-box;
  filter: drop-shadow(8px 8px 5px gray);
}
ul {
  display: flex;
  flex-wrap: wrap;
  list-style-type: none;
  padding: 0;
}
li {
  flex-grow: 1;
  flex-basis: 300px;
  text-align: center;
  padding: 30px;
  border: 1px solid #222;
  border-radius: 5px;
  margin: 10px;
}
h2 {
  cursor: pointer;
}
</style>