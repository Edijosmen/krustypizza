<template>

    <div id="nav">
        <router-link to="/inicio">Inicio</router-link> |
        <router-link to="/login">Ingresar</router-link>
    </div>

    <div >
        <div class="container">
            <nav class="border border-dark navbar navbar-light navbar-expand-sm" style="background-color: #f4f9fc;">
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
                </button>

                <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                <div class="navbar-nav mx-auto text-center">
                <a class="nav-link active" href="pizza" tabindex="-1" aria-disabled="true">Pizzas</a>
                <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Bebidas</a>
                <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Postres</a>
                </div>
                </div>
            </nav>
        </div>
        
        <div class=" container-fluid cabeza">
            <section class = "row justify-content-center">
                <div class = " col-sm-12 col-md-6">
                    <div class=" container carucel">
                        <div id="carouselExampleIndicators" class="carousel slide" data-ride="carousel">
                            <ol class="carousel-indicators">
                                <li data-target="#carouselExampleIndicators" data-slide-to="0" class="active"></li>
                                <li data-target="#carouselExampleIndicators" data-slide-to="1"></li>
                                <li data-target="#carouselExampleIndicators" data-slide-to="2"></li>
                            </ol>
                            <div class="carousel-inner">
                                <div class="carousel-item active">
                                    <img src="../assets/img/pizzainicio.jpg" class="d-block w-100" alt="...">
                                </div>
                                <div class="carousel-item">
                                    <img src="../assets/img/bebidas.jpg" class="d-block w-100" alt="...">
                                </div>
                                <div class="carousel-item">
                                    <img src="../assets/img/postremaracuya.jpg" class="d-block w-100" alt="...">
                                </div>
                            </div>
                            <a class="carousel-control-prev" href="#carouselExampleIndicators" role="button" data-slide="prev">
                                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                                <span class="sr-only">Previous</span>
                            </a>
                            <a class="carousel-control-next" href="#carouselExampleIndicators" role="button" data-slide="next">
                                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                                <span class="sr-only">Next</span>
                            </a>
                        </div>
                    </div>
                </div>
            </section>
        </div>
        <section class="container content">
            <div class="row">
                <div class="col-sm-12 col-md-4">
                    <div>
                        <div class="card" style="width: 18rem;">
                                <img src="../assets/img/fondo2.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                    <h5 class="card-title">Pizzas</h5>
                                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    <a href="#" class="btn btn-primary">Go somewhere</a>
                                </div>
                            </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-4">
                    <div>
                        <div class="card" style="width: 18rem;">
                                <img src="../assets/img/choco.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                    <h5 class="card-title">Bebidas</h5>
                                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    <a href="#" class="btn btn-primary">Go somewhere</a>
                                </div>
                            </div>
                    </div>
                </div>
                <div class="col-sm-12 col-md-4">
                    <div>
                        <div class="card" style="width: 18rem;">
                                <img src="../assets/img/postrecillo.jpg" class="card-img-top" alt="...">
                                <div class="card-body">
                                    <h5 class="card-title">Postres</h5>
                                    <p class="card-text">Some quick example text to build on the card title and make up the bulk of the card's content.</p>
                                    <a href="#" class="btn btn-primary">Go somewhere</a>
                                </div>
                            </div>
                    </div>
                </div>
            
            </div>
        </section>            
   </div>
   <div class="">
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

<style >
/*
    #carouselExampleIndicators{
        width: 600px;
        height: 380px;
        margin: 80px 5px;
    }
    
    .Inicio_Krusty{
        background-image: url("../assets/img/fondopizzados.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        margin: 0;
        padding: 0;
    }
    */
    .cabeza{
        background-image: url("../assets/img/cabezarsel.jpg");
        background-repeat: no-repeat;
        background-size: cover;
        margin: 0;
        padding-top: 20px;
        padding-bottom: 20px;
        margin-bottom: 20px;
    }

    #nav{
        background:#F7C700;
    }

    .carucel{
        background:#fcf6dc;
        border-radius: 10px;
        box-shadow: 0px 0px 10px 0px #000;
        
    }

    .carousel-inner img{
        width: 100%;
        height: 100%;
    }
    
</style>