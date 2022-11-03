<template>
  <button class="btn" @click="onClick()" :style="{ background: color }">
    {{ text }}
  </button>
</template>

<script>
export default {
  name: "Button",
  props: {
    color: {
      type: String,
      default: "green",
    },
    text: String,
  },
  methods: {
    onClick() {
      console.log("on Click");
    },
  },
};
</script>

<style></style>
