<template>
  <section class="todoapp">
    <header class="header">
      <h1>Tarefas</h1>
      <InputTask />
    </header>
  </section>
</template>

<script>
import InputTask from "./components/InputTask.vue";

export default {
  name: "app",
  components: {
    InputTask,
  },
};
</script>

<style>
</style>
