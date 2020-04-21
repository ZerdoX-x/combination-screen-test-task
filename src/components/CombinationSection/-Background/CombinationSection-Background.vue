<template>
  <div class="background">
    <img
      class="background__image"
      src="../../../assets/bg-left.png"
      alt="background image"
    />
    <img
      class="background__image"
      src="../../../assets/bg-right.jpg"
      alt="background image"
    />
  </div>
</template>

<style lang="stylus" scoped>
.background
  left 0
  top 60px
  position absolute
  width 100vw
  display flex
  align-items center
  justify-content space-between
  opacity 0.17

.background__image
  height 650px
  min-width 120px
  @media screen and (max-width: 1090px)
    height 70vw
    &:first-of-type
      transform translateX(-39%)
    &:last-of-type
      transform translateX(33%)
</style>
