<template>
  <div class="parent" :class="class">
    <h3>Component inherit false (with class prop)</h3>
    <div class="child" v-bind="$attrs">
      <h4>v-bind inherit false (with class prop)</h4>
    </div>
  </div>
</template>

<script>
export default {
  props: ['class'],
  inheritAttrs: false,
};
</script>

<style scoped>
.child {
  color: red;
}
</style>
