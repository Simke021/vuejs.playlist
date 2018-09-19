<template>
    <div>
        <form-helper>
          <div slot="form-header">
            <h3>This is the title of the form</h3>
            <p>Information about the form</p>
          </div>

          <div slot="form-fields">
            <input type="text" placeholder="your name" required>
            <input type="password" placeholder="password" required>
          </div>
          <div slot="form-controls">
            <button v-on:clcik="submit">Submit</button>
          </div>
        </form-helper>       
    </div>
</template>

<script>
import formHelper from "./components/formHelper.vue";

export default {
  components: {
    "form-helper": formHelper
  },
  data() {
    return {
      title: "I am dinamic slot title",
      paragraph: "I am the dinamic paragraph text for the slots"
    };
  },
  methods: {}
};
</script>

<style>
</style>