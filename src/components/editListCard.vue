<script setup>
import { ref } from 'vue'

let id = 0

const props = defineProps({
  text1: String,
  text2: String,
  text3: String
})


const newTodo = ref('')
const todos = ref([
  { id: id++, text: props.text1 },
  { id: id++, text: props.text2 },
  { id: id++, text: props.text3 }
  
])

function addTodo() {
  todos.value.push({ id: id++, text: newTodo.value })
  newTodo.value = ''
}

function removeTodo(todo) {
  todos.value = todos.value.filter((t) => t !== todo)
}
</script>

<template>
  <form @submit.prevent="addTodo">
    <input v-model="newTodo">
    <button>Add Todo</button>    
  </form>
  <ul>
    <li v-for="todo in todos" :key="todo.id">
      {{ todo.text }}
      <button @click="removeTodo(todo)">X</button>
    </li>
  </ul>
</template>