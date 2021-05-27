<template>
  <div id="app">
    <Nopage />
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
  color: #2a86e2;
}
</style>
