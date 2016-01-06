<template>
  <input v-model="newTodo" v-on:keyup.enter="addTodo" placeholder="Add a new Todo">
  <ul>
    <li v-for="todo in todos">
      <span>{{ todo.text }}</span>
      <button @click="removeTodo($index)">X</button>
    </li>
  </ul>
</template>

<script>
export default {
  data () {
    return {
      todos: [
        { text: 'Learn JavaScript' },
        { text: 'Learn Vue.js' },
        { text: 'Build Something Awesome' }
      ]
    }
  },
  methods: {
    addTodo () {
      var text = this.newTodo.trim()
      if (text) {
        this.todos.push({ text: text })
        this.newTodo = ''
      }
    },
    removeTodo (index) {
      this.todos.splice(index, 1)
    }
  }
}
</script>