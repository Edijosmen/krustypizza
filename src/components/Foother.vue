<template>
      <footer class=" text-black mt-5" py-4>
            <div class="container">
                <div class=" row">
                        <!--Menú-->
                                <ul class="col-md-4 col-sm-12 list-unstyled">
                                    <h3>Sobre Nosotros</h3>
                                    <p>Somo un negocio de comida rápida para que las personas disfruten de una buena comida, contamos con un ambiente sano y agradable para que pases en familia. 
                                        Estamos ubicados 
                                        Barrio los prados
                                        Carrera-33-BF
                                        
                                    </p>
                                    <p>Tel:312456345</p>
                                    
                                </ul>
                                <ul class="col-md-4 col-sm-12 list-unstyled">
                                    <li class="font-weight-bold text-uppercase">Productos</li>
                                    <li><a href="#" class="text-reset">bebidas</a></li>
                                    <li><a href="#" class="text-reset">Comidas Rapidas</a></li>
                                    <li><a href="#" class="text-reset">Prostres</a></li>
                                    
                                </ul>

                                <ul class="col-md-4 col-sm-12 list-unstyled">
                                    <li class="font-weight-bold text-uppercase">Ayuda</li>
                                    <li><a href="#" class="text-reset">cuales son nuestros servicios</a></li>
                                    <li><a href="#" class="text-reset">como puedo pedir mi order</a></li>
                                </ul>  
                     
                </div>     
                <div class="footer-cont">
                    © 2020 Krosty-Pizzaa
                </div>         

            </div>
        </footer>  
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
footer{
    background:#d5ac00;
    padding-top:30px;
}
.footer-cont{
    border-top: 1px solid #e5edef;
    padding-top:10px;
    padding-bottom: 10px;
}
</style>