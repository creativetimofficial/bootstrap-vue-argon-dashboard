<template>
  <b-breadcrumb-item :active="active">
    <slot></slot>
  </b-breadcrumb-item>
</template>
<script>
export default {
  name: 'breadcrumb-item',
  props: {
    active: {
      type: Boolean,
      default: false,
      description: 'Whether breadcrumb item is active'
    }
  }
};
</script>
<style></style>
