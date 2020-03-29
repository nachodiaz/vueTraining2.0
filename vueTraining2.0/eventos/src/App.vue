<template>
  <div id="app">
    <Navegacion />
    <Contenido />
  </div>
</template>

<script>
import Contenido from './components/Contenido.vue'
import Navegacion from './components/Navegacion.vue'

export default {
  name: 'App',
  components: {
    Navegacion,
    Contenido
  }
}
</script>

<style>
#app {

}
</style>
