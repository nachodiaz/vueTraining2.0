<template>
    <div class="MiComponente">
        <div class="container">
            <h1>Libros</h1>
            <br>
            <h1>{{libro.titulo}}</h1>
            <h2>{{libro.autor}}</h2>
            <p>{{libro.comentarios.user}}</p>
            
            <h1>{{libro2.titulo}}</h1>
            <h2>{{libro2.autor}}</h2>
        </div>
    </div>
</template>

<script>
export default {
    name: 'MiComponente',
    data(){
        return {
            libro: {
                autor: "Donald Normam",
                titulo: "Psicología de los objetos cotidianos",
                comentarios: {
                    user : 'Excelente libro'
                }
            },
            libro2: {
                autor: "Dieter Rams",
                titulo: "less bus better",
                comentarios: {
                    user : 'Excelente libro'
                }
            }
        }
    }

}
</script>

<style lang="">
   
</style>