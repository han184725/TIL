<template>
  <div>
    <ul>
      <li v-for="(todo, idx) in this.$store.state.todos" :key="`todo-${idx}`">
        <span :class="{completed: todo.completed}" @click="toggleTodo(idx)">
          {{todo.item}}
        </span>
        <i class="fa-solid fa-minus removeIcon" @click="removeTodo(todo, idx)"></i>
      </li>
    </ul>
  </div>
</template>

<script>
export default {
  methods: {
    removeTodo(todo, idx){
      const obj = {
        todoItem: todo.item,
        idx: idx,
      }
      this.$store.commit('removeTodo', obj)
    },
    toggleTodo(idx){
      this.$store.commit('toggleTodo', idx)
    },
  },
}
</script>

<style>
li {
  height: 30px;
  display: flex;
}
.removeIcon{
  margin-left: auto;
  color: red;
}
.completed{
  text-decoration: line-through;
  color: grey;
}
</style>