<template>
  <div class="advantage-card">
    <div class="advantage-card__icon">
      <slot />
    </div>
    <h3 class="advantage-card__title">{{ title }}</h3>
    <p class="advantage-card__subtitle">{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  name: "AdvantageCard",
  props: {
    title: { type: String, required: true },
    subtitle: { type: String, required: true }
  }
};
</script>

<style lang="stylus" scoped>
@import url('https://fonts.googleapis.com/css2?family=Open+Sans:wght@400;700&display=swap');
.advantage-card
  display flex
  flex-wrap wrap
  flex-basis 250px
  font-family "Open Sans"
  color #FFFFFF
  margin 0 15px
  @media screen and (max-width: 1220px)
    margin 40px calc(6%)
    flex-grow 1
    min-width 250px
  @media screen and (max-width: 756px)
    max-width 270px

.advantage-card__icon
  @media screen and (max-width: 1220px)
    width 35%

.advantage-card__title
  font-size 24px
  line-height 32px
  @media screen and (max-width: 1220px)
    width 65%
    font-size 16px
    line-height 22px

.advantage-card__subtitle
  flex-grow 1
  opacity 0.5
  font-size 16px
  line-height 24px
  @media screen and (max-width: 1220px)
    text-align center
    font-size 14px
    line-height 22px
</style>
