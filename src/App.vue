<template>
  <div id="app">
    <Todos v-bind:todos="todos" />
  </div>
</template>

<script>
import Todos from './components/Todos'

export default {
  name: 'App',
  components: {
    Todos
  },
  data (){
    return {
      todos: [
        {
          id: 1,
          title: 'Learn JavaScript',
          completed: false
        },
        {
          id: 2,
          title: 'Learn Vue',
          completed: false
        },
        {
          id: 3,
          title: 'Build something awesome',
          completed: false
        }
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

body {
  font-family: Arial, Helvetica, sans-serif;
  line-height: 1.5;
}
</style>
