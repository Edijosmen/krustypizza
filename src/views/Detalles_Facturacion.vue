<template>
    <div class="container">
        <div class="row">
                <div class="col">
                Primera Columna
                </div>
        </div>
        <div class="row">
             <div class="col">
                 Segunda Columna
            </div>
        </div>   
        <!--COLUMNA FORMULARIO DE FACTURACIÓN-->
        <div class="row">
            <div class="col-md-6">
                Tercera Columna 
                <div class="container facturacion">
                                <!--FORMULARIO PVTO-->    
                                <form class="text-left">
                                    <p>DETALLES DE FACTURACIÓN</p>
                                    <div class="form-row">
                                        <div class="form-group col-sm-6">
                                            <label for="inputEmail4">Nombres</label>
                                            <input type="nombres" class="form-control" id="inputNombres4" placeholder="Nombres">
                                        </div>
                                        <div class="form-group col-sm-6">
                                            <label for="inputPassword4">Apellidos</label>
                                            <input type="apellidos" class="form-control" id="inputApellidos4" placeholder="Apellidos">
                                        </div>
                                    </div>
                                    <div class="form-row">
                                        <div class="form-group col-sm-6">
                                        <label for="inputEmail4">Email</label>
                                        <input type="email" class="form-control" id="inputEmail4" placeholder="Email">
                                        </div>
                                        <div class="form-group col-md-6">
                                        <label for="inputPassword4">Teléfono</label>
                                        <input type="telefono" class="form-control" id="inputTelefono4" placeholder="Teléfono">
                                        </div>
                                    </div>
                                    <div class="form-row">
                                        <div class="form-group col-md-12">
                                            <label for="inputAddress2">Dirección</label>
                                            <input type="text" class="form-control" id="inputAddress2" placeholder="Apartment, studio, or floor">
                                        </div>
                                    </div>
                                    <div class="form-group">
                                        <div class="form-group col-md-12">
                                        <label for="inputCity">Ciudad</label>
                                        <select id="inputCity" class="form-control">
                                            <option selected>Seleccionar...</option>
                                            <option>...</option>
                                        </select>
                                        </div>
                                    </div>
                                    <div class="form-group">
                                        <div class="form-check">
                                        <input class="form-check-input" type="checkbox" id="gridCheck">
                                        <label class="form-check-label" for="gridCheck">
                                            Acepto la Política de Tratamiento de Datos*
                                        </label>
                                        </div>
                                    </div>
                                    <!--<button type="submit" class="btn btn-primary">Realizar Pedido</button>-->
                                </form>
                </div> 
                

            </div>
            <!--COLUMNA DETALLE DE PEDIDO-->
           <div class="col-md-6">
                Cuarta Columna 
                <div class="container facturacion">
                   
                     <div class="card text-center">
                            <div class="card-header">
                                TU PEDIDO
                            </div>
                            <div class="card-body">
                                <div class="row">
                                    <div class="col-md-6">
                                       <span class="producto">PRODUCTO</span>     
                                    </div>
                                    <div class="col-md-6">
                                       <span class="producto text-align:right">SUBTOTAL</span>     
                                    </div>

                                </div>
                                 <div class="row">
                                    <div class="col-md-6 mt-4">
                                       <span class="producto">TOTAL</span>     
                                    </div>

                                </div>
                                <div class="row">
                                    <div class="col mt-5">
                                       <div class="form-check">
                                            <input class="form-check-input" type="checkbox" id="gridCheck">
                                            <label class="form-check-label" for="gridCheck">
                                                Pago en efectivo
                                            </label>
                                        </div>    
                                    </div>
                                </div>
                                  <div class="row">
                                    <div class="col">
                                       <div class="form-check">
                                            <input class="form-check-input" type="checkbox" id="gridCheck">
                                            <label class="form-check-label" for="gridCheck">
                                                He leído y estoy de acuerdo con los Términos y Condiciones
                                            </label>
                                        </div>    
                                    </div>
                                </div>
                                <!-- <h5 class="card-title">Special title treatment</h5>
                               <p class="card-text">With supporting text below as a natural lead-in to additional content.</p>-->
                                <a href="#" class="btn btn-primary mt-4">Realizar Pedido</a>
                            </div>
                           
                    </div>
                </div> 
                

            </div>
                    
        </div>
       
    </div>
</template>

<script>
export default {
  name: "Foother",
  props: {
    msg: String,
  },
};
</script>

<style scoped>
     .facturacion{
        margin-top: 150px;
    }

    
   
</style>