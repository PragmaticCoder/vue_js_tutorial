<template>
  <div>
    <div v-bind:key="todo.id" v-for="todo in todos">
      <TodoItem v-bind:todo="todo" v-on:del-todo="$emit('del-todo', todo.id)" />
    </div>
    <AddTodo />
  </div>
</template>

<script>
import AddTodo from "./AddTodo.vue";
import TodoItem from "./TodoItem.vue";

export default {
  name: "Todos",
  components: {
    TodoItem,
    AddTodo
  },
  props: ["todos"]
};

</script>

<style scoped></style>
