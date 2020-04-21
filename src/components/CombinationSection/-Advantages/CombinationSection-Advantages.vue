<template>
  <div class="advantages-wrapper">
    <div class="advantages">
      <slot />
    </div>
    <div class="advantages__indent" />
  </div>
</template>

<style lang="stylus" scoped>
.advantages-wrapper
  display flex
  flex-direction column
  align-items: center

.advantages
  display flex
  flex-wrap wrap
  justify-content space-between
  margin 0 -30px
  width calc(100% - 60px)
  @media screen and (max-width: 756px)
    justify-content center

.advantages__indent
  max-height 100px
  height 6.9444vw
  min-height 55px
</style>
