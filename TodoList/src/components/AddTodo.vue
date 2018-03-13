<h1>Todo List</h1>
<!-- 调用子组件，并使用 v-on 监听 add 方法 -->
<!-- 当 add 事件触发时，就调用当前组件 addTodo 这个方法 -->
<todo-add v-on:add="addTodo"></todo-add>
<ul class="todos">
<!-- // 调用子组件 -->

<script>
  // 引入子组件
  import TodoAdd from './TodoAdd.vue'
  export default {
    name: 'TodoList',
    components: {
      TodoAdd
    },
    // ...
    methods: {
      // ...
      // 添加新的 todo
      addTodo() {
        this.todos.push({
          text: todo,
          isCompleted: false
        })
      }
    }
  }
</script>