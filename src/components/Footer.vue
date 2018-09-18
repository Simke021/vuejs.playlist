<template>
    <footer>
        <p>{{ copyright }}</p>
    </footer>
</template>
<script>
export default {
  data() {
    return {
      copyright: "Copyright 2018 Vue Ninjas :)"
    };
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
}
p {
  color: lightgreen;
  text-align: center;
  text-transform: uppercase;
}
</style>