<template>
  <div id="app">
    <input v-model="a" />
    +
    <input v-model="b" />
    <v-btn color="blue" @click="add">equals</v-btn>
    {{result}}
  </div>
</template>


<script>
import Vue from "vue";
export default Vue.extend({
  el: "#app",
  data: () => ({
    a: "0",
    b: "0",
    result: 0
  }),
  methods: {
    add: function() {
      this.result = parseInt(this.a) + parseInt(this.b);
    }
  }
});
</script>
