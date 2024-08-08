<template>
  <div class="parent" :class="$attrs.class" :style="$attrs.style">
    <h3>Component inherit false (with $attrs.class)</h3>
    <div class="child" v-bind="compatAttrs">
      <h4>v-bind inherit false (with $attrs.class)</h4>
    </div>
  </div>
</template>

<script>
export default {
  inheritAttrs: false,
  computed: {
    compatAttrs(i) {
      const attrs = { ...this.$atts };
      delete attrs.class;
      delete attrs.style;
      return attrs;
    },
  },
};
</script>

<style scoped>
.child {
  color: red;
}
</style>
