<script lang="ts" setup>
defineEmits(["update:count"]);
</script>

<template>
  <button @click="$emit('update:count')">
    <slot></slot>
  </button>
</template>
