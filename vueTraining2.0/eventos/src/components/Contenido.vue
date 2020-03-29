<template>
    <div>
        <div class="jumbotron">
            <h1 class="display-4">Aprendiendo Vuejs</h1>
        </div>

        <Opcion1 />
    </div>
</template>

<script>
import Opcion1 from './Opcion1.vue'

export default {
    name:'Contenido',
    components:{
      Opcion1
    },
    data(){
        return {

        };
    },
    
}
</script>

<style>

</style>
