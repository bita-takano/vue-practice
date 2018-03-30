<template>
  <div class="top">
    <h2>ここはホーム画面です</h2>
    <todo-list :todos="todos"></todo-list>
  </div>
</template>

<script>
import TodoList from '@/components/TodoList';
import data from '../static/data.json';

export default {
  name: 'Top',
  components:
  {
    'todo-list': TodoList,
  },
  data() {
    return {
      todos: data.todos,
    };
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.top{
  margin: 30px 10px;
  text-align: center;
}
</style>
