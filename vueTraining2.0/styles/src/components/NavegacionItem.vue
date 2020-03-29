<template>
  <div>
        <li class="nav-item"  v-bind:class="{active : mostrarActivo}">
          <a class="nav-link"   v-bind:href="navegacionData.url"> {{navegacionData.titulo}} <span class="sr-only">(current)</span></a>
        </li>
  </div>
</template>

<script>
export default {
    name:'NavegacionItem',
    data(){
        return {
            mostrarActivo: true,
            colorAzul: '#0D47A1',
      };
    },
    props: {
        navegacionData: Object
    }
}
</script>

<style>

</style>