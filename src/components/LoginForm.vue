<template>
  <v-form v-model="valid">
    <div class="my-2">
      <v-btn color="primary" @click="login">Login</v-btn>
    </div>
  </v-form>
</template>

<script>
import axios from 'axios';

export default {
  methods: {
    login() {
      let s = new FormData();
      s.set("username", "eden")
      s.set("passwd", "123")
      confirm("ok")
      axios.post("/login", s);
    }
  },
  data: () => ({})
};
</script>
