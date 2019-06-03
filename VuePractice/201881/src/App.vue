<template>
  <div id="app">
  <h1>{{ title }}</h1>  
  <ul>
    <li v-for="(todo,index) in todos" :id="index">
      <label>{{ index + 1 }}.{{ todo.value }}</label>
    </li>
  </ul>
  </div>
</template>

<script>
  export default{
    name: 'app',
    data () {
      return {
        title : "Vue-todos",
        todos : [
          { value: "read a book", done: false },
          { value: "exercise", done: true },
          { value: "write a article", done: true }
        ]
      }
    }
  }
</script>

<style></style>
