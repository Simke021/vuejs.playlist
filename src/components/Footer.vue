<template>
    <footer>
        <p>{{ copyright }} | {{ title }} :)</p>
    </footer>
</template>
<script>
import { bus } from "../main";

export default {
  props: {
    title: {
      type: String
    }
  },
  data() {
    return {
      copyright: "Copyright 2018"
    };
  },
  created() {
    bus.$on("titleChanged", data => {
      this.title = data;
    });
  }
};
</script>
<style scoped>
footer {
  background: #222;
  padding: 10px;
  height: 50px;
  position: fixed;
  left: 0;
  bottom: 0;
  width: 100%;
  border-top: 3px solid lightgreen;
}
p {
  color: lightgreen;
  text-align: center;
  text-transform: uppercase;
}
</style>