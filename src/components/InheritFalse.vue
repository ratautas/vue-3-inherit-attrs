<template>
  <div class="parent">
    <h3>Component inherit false</h3>
    <div class="child" v-bind="$attrs">
      <h4>v-bind inherit false</h4>
    </div>
  </div>
</template>

<script>
export default {
  inheritAttrs: false,
};
</script>

<style scoped>
.child {
  color: red;
}
</style>
