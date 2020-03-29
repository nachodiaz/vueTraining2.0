<template>
    <div class="container" id="MiComponente">
        <h1>Lista de Colores</h1>
        <ul>
            <li v-for="color in colores" :key="(color, index)">
              Nombre en español: {{color.nombreEnEspañol}}
            </li>
            <hr>
             <li v-for="color in colores" :key="(color, index)">
              Nombre en español: {{color.nombreEnIngles}}
            </li>
        </ul>
        
    </div>
</template>

<script>
export default {
    name: "MiComponente",
    data(){
        return {
            colores:[
                {nombreEnEspañol: "rojo", nombreEnIngles:"red" },
                {nombreEnEspañol: "amarillo", nombreEnIngles:"yewllow" },
                {nombreEnEspañol: "rosado", nombreEnIngles:"pink" },
                {nombreEnEspañol: "azul", nombreEnIngles:"blue" },
            ]
        };
    }
}
</script>

<style>

</style>