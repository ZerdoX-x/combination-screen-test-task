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

.app__content
  flex-grow 1

.app__indent
  width 6.9444vw
  min-width 20px
  z-index 50
</style>
