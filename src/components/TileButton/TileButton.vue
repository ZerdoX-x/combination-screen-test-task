<template>
  <button class="tile-button">
    <span tabindex="-1" class="tile-button__content">
      Join
    </span>
  </button>
</template>

<style lang="stylus" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
.tile-button
.tile-button__content
  transition background-color 0.3s, color 0.3s
  display flex
.tile-button
  cursor pointer
  background-color #005be9
  border none
  font-family "Open Sans"
  color #FFFFFF
  text-transform uppercase
  font-weight bold
  max-width 280px
  width 87.5vw
  min-width 260px
  height 64px
  margin 0 auto
  align-self center
  padding 0
  &:hover
    background-color #166efa
  &:focus > .tile-button__content
    outline none
    background-color #166efa
    color #95ff00

.tile-button__content
  width 100%
  height 100%
  align-items center
  justify-content center

.tile-button:focus
.tile-button__content:focus
  outline none
</style>
