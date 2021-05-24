<template>
  <div class="password-shadow">
    <ModuleTransition>
      <h3 class="title" v-show="lexShowModule">
        {{ isPage ? $frontmatter.title : $site.title || $localConfig.title }}
      </h3>
    </ModuleTransition>
    <ModuleTransition delay="0.08"></ModuleTransition>
    <ModuleTransition delay="0.16"></ModuleTransition>
    <ModuleTransition delay="0.24"></ModuleTransition>
  </div>
</template>

<script>
import ModuleTransition from "../components/ModuleTransition";

export default {
  components: { ModuleTransition },
};
</script>

<style>
</style>