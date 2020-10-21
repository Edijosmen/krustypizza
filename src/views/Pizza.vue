<template>
    <Navbaru/>
        <div class="container">
            <nav class="navbar navbar-light navbar-expand-sm" style="background-color: #f4f9fc;">
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
                </button>

                <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                <div class="navbar-nav mx-auto text-center">
                <a class="nav-link active" href="" tabindex="-1" aria-disabled="true">Pizzas</a>
                <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Bebidas</a>
                <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Postres</a>
                </div>
                </div>
            </nav>
        </div>
        <!--seccion de domicilio -->
    <section class="lista Pizza domicilio">
        <div class="container domicilio">
            <div class="row justify-content-center">
            <div class="col-sm-6 col-md-6">
                <div class="row">
                        <div class="col-sm-12 col-md-6 ">
                            <i class="fas fa-bicycle fa-10x bike"></i>
                        </div>
                        <div class="col-sm-12 col-md-6">
                            <div class="card" style="width: 18rem;">
                            <div class="card-header font-weight-bold">
                                Horario de Domicilio
                            </div>
                            <ul class="list-group list-group-flush">
                                <li class="list-group-item">Domingo a Jueves </li>
                                <li class="list-group-item">11:30 AM a 10:30 PM</li>
                                <li class="list-group-item">Viernes a Sabados</li>
                                <li class="list-group-item">11:0 AM a 11:30 PM</li>
                            </ul>
                            </div>
                        </div>
                </div>
            </div>
            </div>
        </div>

    </section>
    <!-- contenido de la lista productos-->
    <section>
        <div class="container">
            <div class="contend">
            <div class="row">
                <div class="col-sm-12 col-md">
                    <div>
                        <div class="card" >
                                <img src="../assets/img/fondo2.jpg" class="card-img-top" >
                                <div class="card-body">
                                    <h5 class="card-title">Pizzas</h5>
                                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    <a href="#" class="btn btn-danger">Go somewhere</a>
                                </div>
                            </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md">
                    <div>
                        <div class="card" >
                                <img src="../assets/img/choco.jpg" class="card-img-top" >
                                <div class="card-body">
                                    <h5 class="card-title">Bebidas</h5>
                                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    <a href="#" class="btn btn-danger">Go somewhere</a>
                                </div>
                            </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md">
                    <div>
                        <div class="card" >
                                <img src="../assets/img/postrecillo.jpg" class="card-img-top" >
                                <div class="card-body">
                                    <h5 class="card-title">Postres</h5>
                                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    <a href="#" class="btn btn-danger ">Go somewhere</a>
                                </div>
                            </div>
                    </div>
                </div>
            
            </div>
            </div>
        </div>
    </section>
     <Foother/>

</template>
   
<script>
import Foother from '@/components/Foother.vue'
import Navbaru from '@/components/Navbaru.vue'
export default {
    components: {
    Navbaru,
    Foother
  }
}
</script>

<style scoped>
.contend{
    margin-top: 20px;
    border-top: 5px solid #e5edef;
    padding-top:20px;
}
.domicilio{
   background-image: url("../assets/img/banner2.jpg");
    padding-top:20px;
    padding-bottom:20px;
    background-repeat: no-repeat;
    background-size: cover;
}
.bike{
    color: #F7C700;
}
.card-header{
    background: #DC3545;
    color: white;
}
.bbtn{
     background:#F52F41;
    color:white
}
</style>