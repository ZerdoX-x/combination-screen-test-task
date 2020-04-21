<template>
  <div id="app">
    <div class="app-wrapper">
      <div class="app__indent app__indent_left" />
      <main class="app__content">
        <combination-section />
      </main>
      <div class="app__indent app__indent_right" />
    </div>
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
  background rgba(9, 7, 39, 0.88)

.app-wrapper
  background rgba(9, 12, 19, 0.83)
  width 100%
  display flex

.app__content
  flex-grow 1

.app__indent
  width 6.9444vw
  min-width 20px
  z-index 50
</style>
