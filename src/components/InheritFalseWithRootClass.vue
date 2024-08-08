<template>
  <div class="parent" :class="rootClass">
    <h3>Component inherit false (and rootClass)</h3>
    <div class="child" v-bind="$attrs">
      <h4>v-bind inherit false (and rootClass)</h4>
    </div>
  </div>
</template>

<script>
export default {
  inheritAttrs: false,
  props: ['rootClass'],
};
</script>

<style scoped>
.child {
  color: red;
}
</style>
