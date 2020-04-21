<template>
  <div id="app">
    <combination-section />
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
</style>
