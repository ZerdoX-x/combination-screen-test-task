<template>
  <h1 class="heading">
    <slot />
  </h1>
</template>

<style lang="stylus" scoped>
@import url('https://fonts.googleapis.com/css2?family=Vollkorn&display=swap')

.heading
  align-self center
  text-align center
  font-weight normal
  font-style normal
  color #FFFFFF
  font-size calc(157% + 2.03vw)
  line-height 66px
  font-family Vollkorn
  width 70.9375vw
</style>
