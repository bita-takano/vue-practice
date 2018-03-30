<template>
  <div class="todolist">
    <table border="1">
      <tr v-for="todo in todos" :key="todo.id" class="todoitem">
        <td class="id">{{ todo.id }}</td>
        <td class="text">{{ todo.text }}</td>
      </tr>
    </table>
  </div>
</template>

<script>
export default {
  name: 'TodoList',
  props: [
    'todos',
  ],
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.todolist{
  width: 500px;
  margin: 0 auto;
  text-align: center;
}
.id{
  width: 100px;
}
.text{
  width: 400px;
}
</style>
