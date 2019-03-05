<template>
  <div id="app">
    <div id="root">
      <div class="todo-container">
        <div class="todo-wrap">
          <TodoTop />
          <TodoList />
          <TodoBottom />
        </div>
      </div>
    </div>
  </div>
</template>

<script>
// 1、引入组件
import TodoTop from './components/TodoTop.vue'
import TodoList from './components/TodoList.vue'
import TodoBottom from './components/TodoBottom.vue'

export default {
name: 'App',
// 2、映射组件标签，可以写多个
  components: {
    TodoTop,
    TodoList,
    TodoBottom
  }
}
</script>

<style>
#app {
  font-family: 'Avenir', Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
.todo-container {
  width: 600px;
  margin: 0 auto;
}
.todo-container .todo-wrap {
  padding: 10px;
  border: 1px solid #ddd;
  border-radius: 5px;
}
</style>
