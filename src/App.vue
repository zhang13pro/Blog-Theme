<template>
  <div id="app">
    <Nopage />
    <!-- <img alt="Vue logo" src="./assets/logo.png" width="25%" /> -->
  </div>
</template>

<script>
import Nopage from "./.vuepress/theme/layouts/404";

export default {
  name: "App",
  components: {
    Nopage,
  },
};
</script>

<style>
#app {
  font-family: "Avenir", Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
