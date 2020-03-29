<template>
  <div id="app">
    <Home />
    <Navegacion />
    <br>
    <div class="row">
      <Contenido />
    </div>
  </div>
</template>

<script>
import Home from './components/Home.vue'
import Navegacion from './components/Navegacion.vue'
import Contenido from './components/Contenido.vue'


export default {
  name: 'App',
  components: {
    Home,
    Navegacion,
    Contenido
 }
}
</script>

<style>

  
</style>
