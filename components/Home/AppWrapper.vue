<template>
  <div class="app-wrapper">
    <AppHeader />
    <TodoList />
  </div>
</template>

<script>
import AppHeader from './AppHeader'
import TodoList from './TodoList'

export default {
  components: {
    AppHeader,
    TodoList
  }
}

</script>

<style scoped>
.app-wrapper {
  border-radius: 30px;
  max-width: 500px;
  width: 100%;
  background-color: #FFFFFF;
  height: 50vh;
  /*height: auto;*/
  padding: 50px;
}
</style>
