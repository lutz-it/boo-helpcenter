<template>
  <div class="px-3 py-2 text-sm rounded-full shadow flex items-center">
    <svg class="mr-2" style="width: 18px; height: 18px" viewBox="0 0 24 24">
      <path :fill="color" :d="d" />
    </svg>
    {{ label }}
  </div>
</template>

<script>
export default {
  props: {
    label: {
      type: String,
      default: "",
    },
    d: {
      type: String,
      default: "",
    },
    color: {
      type: String,
      default: "currentColor",
    },
  },
};
</script>

<style>
</style>