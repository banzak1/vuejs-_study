<template>
  <section class="todoapp">
    <header class="header">
      <h1>Tarefas</h1>
      <InputTask />
      <TaskList :todo-list="tasks" />
    </header>
  </section>
</template>

<script>
import InputTask from "./components/InputTask.vue";
import { Task } from "./models/Taks";
import TaskList from "./components/TaskList.vue";

let tasks = [];
let task = new Task();
task.id = 0;
task.completed = false;
task.title = "Tarefa";
tasks.push(task);
task.id++;
tasks.push(task);
task.id++;
tasks.push(task);


export default {
  name: "app",
  components: {
    InputTask,
    TaskList,
  },
  data() {
    return {
      tasks: tasks,
    };
  },
};
</script>

<style>
</style>
