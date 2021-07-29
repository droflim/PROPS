
<template>
  <div>
    <Todo :title="'Lista de Tareas'" />
  </div>
</template>

<script>
import Todo from '@/components/Todo.vue'
export default {
  name: 'App',
  components: {
    Todo,
  },
}
</script>
