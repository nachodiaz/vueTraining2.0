<template>
  <div >
    <nav class="navbar navbar-expand-lg navbar-dark bg-dark" >
    <a class="navbar-brand" href="#">IDUXU</a>
    <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
    </button>

        <div class="collapse navbar-collapse" id="navbarSupportedContent">
        
        <ul class="navbar-nav mr-auto ">
          
          <NavegacionItem :navegacionData="item" v-for="(item, index) in itemsNavegacion" :key='index' />
 
        </ul>

        <form class="form-inline my-2 my-lg-0">
        <input class="form-control mr-sm-2" type="text" placeholder="Nombre de Usuario" aria-label="Search">
        <input class="form-control mr-sm-2" type="password" placeholder="Contraseña" aria-label="Login">
        <button class="btn btn-outline-success my-2 my-sm-0" type="submit">Login</button>

        </form>
        
      </div>
    </nav>
  </div>
</template>

<script>
import NavegacionItem from './NavegacionItem'

export default {
    name:'Navegacion',
    components:{
      NavegacionItem
    },
    data(){
      return {
       itemsNavegacion:[
         {titulo:'Inicio', url:'/inicio'},
         {titulo:'Planes', url:'/planes'},
         {titulo:'Portafolio', url:'/portafolio'},
         {titulo:'Quiénes Somos', url:'/acercade'},
         {titulo:'Contacto', url:'/contacto'}
       ]
      };
    }
}
</script>

<style>

</style>