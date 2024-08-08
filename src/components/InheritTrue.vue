<template>
  <div class="parent">
    <h3>Component inherit true</h3>
    <div class="child" v-bind="$attrs">
      <h4>v-bind inherit true</h4>
    </div>
  </div>
</template>

<script>
export default {
  inheritAttrs: true,
};
</script>

<style scoped>
.child {
  color: red;
}
</style>
