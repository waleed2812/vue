<template>
  <header>
    <h1>{{title}}</h1>
    <Button text="Add Task" color="green" />
  </header>
</template>

<script>
import Button from "./Button.vue";
export default {
  
  name: "HeaderVue",
  // props: ["title"],
  props: {
    title: {
      type: String,
      default: "Hello World"
    },
  },
  components: {
    Button
  }
};
</script>

<style>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
