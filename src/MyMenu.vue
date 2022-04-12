<template>
  <div @click="onMenuClick">
    <h4>{{ title }}</h4>
    <div>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title"],
  methods: {
    onMenuClick(event) {
      this.$emit("menu-click", event);
    },
  },
};
</script>
<style>
  div {
    cursor: pointer;
  }
</style>
