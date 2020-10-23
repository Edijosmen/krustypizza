<template>
    <div class="container">
        <!--LOGO-->
        <div class="row">
                <div class="col-md-4">
                    <div class="container ">
                        <div class="logo ">
                            <img class="img-fluid img-thumbnail" src="../assets/img/krostyanuncio.jpg">
                        </div>
                    </div>
                </div>
                <div class="col-md-4">
                    <div class="container ">
                        <div class="text-left mt-5 titulogo">
                                <h1 class="align-center">Pizzería Krusty</h1>  
                        </div>
                    </div>
                </div>
                <!--Iconos-->
                <div class="col-sm mt-5 icon">
                    <div class="container user">
                        
                            <a  class=" a-menu font-weight-bold" href=""><i class="far fa-user"></i>  
                                <p>Usuario</p>
                            </a>
                    </div>                  
                </div>
                <div class="col-sm mt-5 icondos">
                    <div class="container car">
                             <a  class=" a-menu font-weight-bold" href=""><i class="fas fa-cart-plus"></i>  
                              <p>Carrito</p>  
                            </a>
                    </div>
                </div>
                 
        </div>
        <!--NAVBAR-->
        <div class="row">
             <div class="col">
               
                   <div class="container">  
                            
                        <nav class="border border-dark navbar navbar-light navbar-expand-sm" style="background-color: #f4f9fc;">
                            <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                            <span class="navbar-toggler-icon"></span>
                            </button>

                            <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                            <div class="navbar-nav mx-auto text-center">
                            <a class="nav-link active" href="#" tabindex="-1" aria-disabled="true">Pedidos</a>
                            <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Ventas</a>
                           
                            </div>
                            </div>
                        </nav>
                    </div>   
            </div>
        </div>   
        <!--COLUMNA PEDIDOS Y VENTAS-->
        <div class="container mt-5">
            <div class="border border-dark card text-center">
                            <div class="card-header">
                                <label for="card-header" class="font-weight-bold">LISTA DE PEDIDOS</label>
                            </div>
                            <div class="card-body">
                                <div class="row mt-5">
                                    <div class="col-sm mt-2">
                                    Date
                                        <input data-provide="datepicker">
                                    </div>
                                    <div class="col-sm">
                            
                                        <select id="inputCity" class="form-control">
                                            <option selected>Seleccionar...</option>
                                            <option>...</option>
                                        </select>
                                    </div>
                                    <div class="col-sm">
                                        <Label class="total">TOTAL</Label>
                                    </div>
                                </div>
                            </div>  
                    </div>
            
            
        </div>
        <br>
       
    </div>
    <div class="">
        <button type="button" class="border border-dark btn btn-success ">Agregar a Ventas</button>
    </div>
    <div>
         <Foother/>
   </div>
</template>

<script>
    import Foother from '@/components/Foother.vue'
    export default {
    name: 'Footer',
    components: {
        Foother
     }
    }
</script>

<style scoped>
    
    .container{
        background: #F0B491;
        background-repeat: no-repeat;
        background-size: cover;
        
    }
    
     .facturacion{
        margin-top: 150px;
    }

  .logo{
      width: 150px;
  }
  .titulogo{
        color: darkgoldenrod;
  }
  .fa-user{
      color: black;
      font-size: 30px;
  }
  .fa-cart-plus{
      color: black;
       font-size: 30px;
       
  }
  .total{
      color: black;
      font-size: 20px;
  }
    .card-header{
        color: black;
    }
 
    
   
</style>