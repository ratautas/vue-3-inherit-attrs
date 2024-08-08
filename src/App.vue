<template>
  <div id="app">
    <InheritTrue class="from-app" />
    <hr />
    <InheritFalseWithProp class="from-app" />
    <hr />
    <InheritFalseWithAttrs class="from-app" />
    <hr />
    <InheritFalseWithRootClass root-class="from-app" />
    <hr />
    <InheritFalse class="from-app" />
    <hr />
  </div>
</template>

<script>
import InheritFalse from './components/InheritFalse.vue';
import InheritFalseWithProp from './components/InheritFalseWithProp.vue';
import InheritFalseWithAttrs from './components/InheritFalseWithAttrs.vue';
import InheritFalseWithRootClass from './components/InheritFalseWithRootClass.vue';
import InheritTrue from './components/InheritTrue.vue';

export default {
  name: 'App',
  components: {
    InheritFalse,
    InheritFalseWithProp,
    InheritFalseWithAttrs,
    InheritFalseWithRootClass,
    InheritTrue,
  },
};
</script>

<style scoped>
body {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
}

.from-app {
  background: yellow;
}
</style>
