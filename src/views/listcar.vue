<template>
    <nav class="navbar navbar-inverse">
        <div class="container-fluid">
            <div class="navbar-header">
                <a href="" class="navbar-brand a-menu font-weight-bold">Krostypizza</a>
            </div>
            <ul class="nav navbar-nav navbar-right"> 
                <li>
                    <a  class=" a-menu font-weight-bold" href="">Usuario <i class="fas fa-user"></i> - </a>
                    <a href=""><i class="fas fa-shopping-cart carico"></i></a>
                </li>
            </ul>
        </div>
    </nav>
    <section class ="content" >
        <div class="container contenido">
            <div class="row">
                <div class="col-md-6 product">
                    <div class="row bord">
                        <div class ="col-sm-6  col-md-5 prod">
                              <label class ="font-weight-bold" for="">Productos</label>
                              <div >
                                    <div class="card-center" style="width: 12rem;">
                                        <img src="../assets/img/postrecillo.jpg" class="card-img-top">
                                        <div class="card-body">
                                            <h5 class="card-title">Postres de leche</h5>
                                        </div>
                                    </div>
                               </div>
                        </div>
                        <div class ="col-sm-6 col-md-2 ">
                             <label class="col font-weight-bold" for="">Precio </label>
                             <label  class="col" for="">$30.000</label>
                        </div>
                        <div class ="col-sm-6 col-md-2"> 
                             <label class="col font-weight-bold" for="">Cantidad</label>
                             <label class="col" for="">4</label>
                        </div>
                        <div class ="col-sm-6 col-md-2 "> 
                             <label class="col font-weight-bold" for="">supTotal</label>
                              <label class="col" for="">$120.000</label>
                        </div>
                    </div>
                    <div class="row bord">
                        <div class ="col-sm-6  col-md-5 prod">
                              <label for="">Productos</label>
                              <div >
                                    <div class="card-center" style="width: 12rem;">
                                        <img src="../assets/img/postrecillo.jpg" class="card-img-top">
                                        <div class="card-body">
                                            <h5 class="card-title">Postres de leche</h5>
                                        </div>
                                    </div>
                               </div>
                        </div>
                        <div class ="col-sm-6 col-md-2 ">
                             <label class="col font-weight-bold" for="">Precio </label>
                             <label  class="col" for="">$30.000</label>
                        </div>
                        <div class ="col-sm-6 col-md-2"> 
                             <label class="col font-weight-bold" for="">Cantidad</label>
                             <label class="col" for="">4</label>
                        </div>
                        <div class ="col-sm-6 col-md-2 "> 
                             <label class="col font-weight-bold" for="">supTotal</label>
                              <label class="col " for="">$120.000</label>
                        </div>
                    </div>
                  
                </div>
                <div class="col-md-6 buy">
                    <div>
                        <div class="row justify-content-center pt-5 pb-5 ">
                           <div class="col-sm-6 col-md-6">
                                
                                        <i class="fas fa-shopping-cart fa-5x shop"></i>
                                    <div class="card-body">
                                        <div class="col-sm-6 col-md-12 ">
                                        <label for="">Total del Compra</label>
                                        </div>
                                        <div class="col-sm-6 col-md-12">
                                        <label class="font-weight-bold" for="">$ 140.000</label>
                                        </div>
                                        <div>
                                            <button class="btn" type="submit">Finalizar compra</button>
                                        </div>
                                            
                                    </div>
                            
                           </div>
                        </div>

                        
                    </div>
                   
                </div>
            </div>
        </div>
    </section>
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
.prod{
    /*padding-right: 90px;*/
}
.contenido{
    background-color: #f2f2f2
}
.content{
    margin-top: 20px;
    border-top: 1px solid #e5edef;
    padding-top:20px;
    
}
nav{
     background:#F7C700;
}
.a-menu{
     color:#25251A;
}
.bord{
    padding-top:10px;
    border-top: 2px solid #e5edef;
}
.compra{
    
    
}
.shop{
    color:#25251A
}
.carico{
    color:#25251A;
}
.buy{
   
}
.product{
    background:#EABF70;
}
.btn{
    background:#F52F41;
    color:white
}
</style>