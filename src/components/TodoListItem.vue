<template>
  <li>
    <div v-if="!tarea.modificable">{{ tarea.$index }}: {{ tarea.texto }}</div><button @click="borrar(tarea)">Eliminar</button>
    
  </li>
</template>

<script>
export default {
  name: 'TodoListItem',
  props: {
    tarea: {
      type: Object,
      required: true,
    },
  },
  methods: {
    borrar(tarea) {
      this.$emit('borrar-tarea', tarea)
    },
  },
}
</script>

<style></style>