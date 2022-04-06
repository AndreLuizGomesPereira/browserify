<template>
  <div>
    <h4>{{ title }}</h4>
    <div>
      <slot></slot>
    </div>
  </div>
</template>

<script>
export default {
  props: ["title"],
};
</script>
<style></style>
