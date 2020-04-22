<template>
  <div class="subtitle-wrapper">
    <div class="subtitle-top-indent" />
    <p class="subtitle">
      <slot />
    </p>
    <div class="subtitle-bottom-indent" />
  </div>
</template>

<style lang="stylus" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
.subtitle-wrapper
  align-self center
  width 60vw

.subtitle
  text-align center
  font-weight normal
  font-style normal
  font-size calc(75% + 0.55vw)
  color #FFFFFF
  font-family "Open Sans"
  line-height calc(170% + 0.05vw)

.subtitle-top-indent
  height 2.6388vw
  min-height 22px

.subtitle-bottom-indent
  height 5.2777vw
  min-height 39px
</style>
