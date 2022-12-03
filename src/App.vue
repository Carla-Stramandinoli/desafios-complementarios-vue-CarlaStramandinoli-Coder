<template>
  <div id="app" class="m-4 px-2">
    <componentes-tabla :alumnos="alumnosPrimero" :estilo="estilo1"/>
    <componentes-tabla :alumnos="alumnosSegundo" :estilo="estilo2"/>
    <componentes-tabla :alumnos="alumnosTercero" :estilo="estilo3"/>
  </div>
</template>

<script>
import ComponentesTabla from './components/ComponentesTabla.vue'

export default {
  name: "app",
  components: {
    ComponentesTabla
  },
  data() {
    return {
      alumnosPrimero: [
        {
          nombre: "Olga Mayor",
          nota: 9
        },
        {
          nombre: "Alejo Acuña",
          nota: 6
        },
        {
          nombre: "Lorena Manso",
          nota: 10
        },
      ],
      alumnosSegundo: [
        {
          nombre: "Leonardo Serra",
          nota: 6
        },
        {
          nombre: "Axel Jimeno",
          nota: 4
        },
        {
          nombre: "Laura Trillo",
          nota: 8
        },
      ],
      alumnosTercero: [
        {
          nombre: "Mariano Orellana",
          nota: 5
        },
        {
          nombre: "Christian Arevalo",
          nota: 7
        },
        {
          nombre: "Emilia Fernndez",
          nota: 7
        },
      ],
      estilo1: ["table", "table-success"],
      estilo2: ["table", "table-dark"],
      estilo3: ["table", "table-striped"],
    }
  }
}
</script>

<style>

</style>
