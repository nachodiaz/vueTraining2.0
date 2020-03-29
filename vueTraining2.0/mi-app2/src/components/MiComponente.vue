<template>
  <div>
      <div class="container">
        <ul>
            <!-- V-for nos sirve para mostrar listas-->
            <!-- v-if nos sirve para mosrar u ocultar -->
            <br>
                <li v-for="x in 1" :key='(x, index)'>
                    Este mensaje se repite una vez 
                    gracias al v-for 
                </li>
                
                <button> Inicio </button>

            <hr>

            <div v-if = "mostrarBoton == 'premium' ">
               
                 <br>
                 Usuario Aunteticado
                <button > Update to premium </button>
            </div>

            <div v-else-if="mostrarBoton">
                Valor encontrado, pero esta incorrecto
            </div>

            <div v-else>
                Valor no encontrado ingrese valor
            </div>

        </ul>
      </div>
  </div>
</template>

<script>
export default {
    name:'app',
    data(){
        return{
            mostrarBoton: "premium" 
        }
    }
}
</script>

<style>
    .container{
        width: 98%;
        margin: 0 auto ;
    }
    li{
        list-style: none;
        display: inline-block;
    }
    button{
        background: green;
        width:120px;
        height:50px;
        border-radius:10px;
        color:white;
        font-size:17px;
        margin-left:14px;
    }
</style>