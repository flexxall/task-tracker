<template>
  <header>
    <h1>{{ title }}</h1>
    <Button text="Add Task" color="green" />
    <!-- <Button text="Update Task" color="burlywood"/> -->
    <!-- <Button text="Delete Task" color="red"/> -->
  </header>
</template>

<script lang="ts">
import { defineComponent } from "vue";
import Button from "./Button.vue";

export default defineComponent({
  name: "Header",
  // props: ["title"]
  props: {
    title: String,
  },
  // props: {
  //   title: {
  //     type: String,
  //     default: "Hello World",
  //   },
  // },
  components: {
    Button,
  },
});
</script>

<style scoped>
header {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-bottom: 20px;
}
</style>
