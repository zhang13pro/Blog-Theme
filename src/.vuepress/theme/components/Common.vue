<template>
  <div
    class="theme-container"
    :class="pageClasses"
    @touchstart="onTouchStart"
    @touchend="onTOuchEnd"
  >
    <div v-if="!absoluteEncryption"></div>
    <div v-else></div>
  </div>
</template>

<script>
import Sidebar from "../components/Sidebar";
import Navbar from "../components/Navbar";
import Password from "../components/Password";
import ModuleTransition from "../components/ModuleTransition";

export default {
  mixins: [ModuleTransition],

  components: { Sidebar, Navbar, Password, ModuleTransition },

  props: {
    sidebar: {
      type: Boolean,
      default: true,
    },
    isComment: {
      type: Boolean,
      default: true,
    },
  },
  data() {
    return {
      isSidebarOpen: false,
      isHasKey: true,
      isHasPageKey: true,
      firstLoad: true,
    };
  },

  computed: {
    absoluteEncryption() {
      return 0;
    },
  },
};
</script>

<style>
</style>