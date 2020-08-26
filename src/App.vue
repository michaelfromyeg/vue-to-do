<template>
  <div class="app">
    <img alt="Post-it logo" src="./assets/logo.png">
    <Header msg="todos"/>
    <TodoEntry />
    <ol>
      <TodoItem
        v-for="todo in todos"
        v-bind:todo="todo.text"
        v-bind:key="todo.id"
      ></TodoItem>
    </ol>
  </div>
</template>

<script>
import Header from './components/Header.vue'
import TodoItem from './components/TodoItem'
import TodoEntry from './components/TodoEntry'

export default {
  name: 'App',
  components: {
    Header,
    TodoItem,
    TodoEntry
  },
  data: function() {
    return {
      todos: [
        {
          text: 'hello world',
          id: 1
        },
        {
          text: 'hello world 2',
          id: 2
        }
      ]
    }
  }
}
</script>

<style>
.app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
