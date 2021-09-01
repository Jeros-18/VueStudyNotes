<template>
  <ul class="todo-main">
    <myItem
      v-for="todoObj in todos"
      :key="todoObj.id"
      :todo="todoObj"
      :checkTodo="checkTodo"
      :deleteTodo="deleteTodo"
    />
  </ul>
</template>

<script>
import myItem from "./myItem";
export default {
  name: "MyList",
  components: { myItem },

  props: ["todos", "checkTodo",'deleteTodo'],
};
</script>

<style>
</style>