<template>
  <div id="app">
    <h1>Todo List</h1>
    <Todos v-bind:todos="todos" />
    <br/>
  </div>

  

</template>



<script>
  import Todos from './components/Todos.vue'

  export default {
    name: 'app',
    components: {
      Todos,
    },
    data() {
      return {
        todos: [
          {
            id: 1,
            title: "Listening",
            isCompleted: false
          },
          {
            id: 2,
            title: "Reading",
            isCompleted: false
          },
          {
            id: 3,
            title: "Sleeping",
            isCompleted: true
          },
        ]
      }
    }
  }
</script>

<style>
  * {
    box-sizing: border-box;
    margin: 0;
    padding: 0;
  }

  #app {
    font-family: 'Roboto', Helvetica, Arial, sans-serif;
    -webkit-font-smoothing: antialiased;
    -moz-osx-font-smoothing: grayscale;
    text-align: center;
    color: #2c3e50;
    margin-top: 60px;
  }
</style>
