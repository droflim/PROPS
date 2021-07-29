<template>
  <div>
    <label>Tarea </label>
    <input type="text" placeholder="Ingrese nueva tarea" v-model="nuevaTarea" />
    <button @click="handleClick">Añadir</button>
  </div>
</template>

<script>
export default {
  name: 'TodoTaskInput',
  data: () => ({
    nuevaTarea: '',
  }),
  methods: {
    handleClick() {
      this.$emit('nueva-tarea', this.nuevaTarea)
      this.nuevaTarea = ''
    },
  },
}
</script>

<style></style>