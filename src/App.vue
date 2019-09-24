<template>
  <div id="app">
    <LoginForm></LoginForm>
  </div>
</template>

<script>
import LoginForm from "./components/LoginForm.vue";

export default {
  name: "app",
  components: {
    LoginForm
  }
};
</script>

<style lang="scss">
@import "assets/sass/stylesheets/main.scss";
</style>
