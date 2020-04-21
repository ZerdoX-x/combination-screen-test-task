<template>
  <div id="app">
    <div class="app__indent app__indent_left" />
    <main class="app__content">
      <combination-section />
    </main>
    <div class="app__indent app__indent_right" />
  </div>
</template>

<script>
import CombinationSection from "./components/CombinationSection/CombinationSection";
export default {
  name: "App",
  components: { CombinationSection }
};
</script>

<style lang="stylus" scoped>
#app
  background #090C13
  display flex
  overflow hidden

.app__content
  flex-grow 1
  max-width 1240px

.app__indent
  flex-grow 1
  min-width 20px
</style>
