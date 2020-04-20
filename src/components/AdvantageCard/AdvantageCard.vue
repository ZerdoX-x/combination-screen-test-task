<template>
  <div>
    <h3>{{ title }}</h3>
    <p>{{ subtitle }}</p>
  </div>
</template>

<script>
export default {
  name: "AdvantageCard",
  props: {
    icon: { type: null, required: true },
    title: { type: String, required: true },
    subtitle: { type: String, required: true }
  }
};
</script>

<style lang="stylus" scoped></style>
