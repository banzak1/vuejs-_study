<template>
  <input
    type="text"
    class="new-todo"
    placeholder="Oque presa ser feito?"
    @keyup.enter="addTask"
  />
</template>

<script>
import { Task } from "../models/Taks.js";

export default {
  data() {
    return {};
  },

  methods: {
    addTask($event) {
      let value = $event.target.value;
      let task = new Task();
      task.completed = false;
      task.title = value;
      console.log(task);
    },
  },
};
</script>

<style scoped>
</style>
