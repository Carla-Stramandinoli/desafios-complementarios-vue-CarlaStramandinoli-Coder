<template>
  <div>
    <table :class="estilo">
      <thead :class="estilo">
        <tr>
          <th>Nombre</th>
          <th>Nota</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="(alumnos, index) of alumnos" :key="index">
          <td>{{ alumnos.nombre }}</td>
          <td>{{ alumnos.nota }}</td>
        </tr>
      </tbody>
    </table>
  </div>
</template>

<script>
export default {
  name: 'ComponentesTabla',
  props: {
    alumnos: Array,
    estilo: Array
  }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>

</style>
