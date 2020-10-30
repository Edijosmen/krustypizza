<template>
  <div>
    <div
      class="card"
      style="width: 18rem;"
    >
      <img
        :src="imagen.img_product"
        class="card-img-top"
        alt="..."
      >
      <div class="card-body">
        <h5 class="card-title">{{imagen.nombre}}</h5>
        <p class="card-text">{{imagen.descripcion}}</p>
        <p class="card-text">${{imagen.precio}}</p>

        <button         
        class="btn btn-primary" 
        @click="agregar_producto()">
        Agregar</button>
      </div>
    </div>
  </div>
</template>

<script>
import axios from 'axios'
export default {
    name: 'Imagen',
    props: ['imagen'],
    data(){
      return {
        estado: true,
        producto: 0,
        total: 0.0,
        id_venta: 1,
        precio_tmp: 0,
        
      }
    },
    methods:{
      agregar_producto(){
        //Creamos el objeto de venta
        if(this.estado){
        axios.post("http://127.0.0.1:8000/ventas/ventas/", {
          total: 5000
        },{
            headers: {
            "Authorization": "JWT " + localStorage.getItem("token")
        }
        }).then((response)=>{           
          console.log(response.data)
        })
        this.estado=false

        }else{
                  //Creamos el objeto de detalleventa

          //algo
        }
        this.producto += 1
        console.log(this.producto)
        console.log(this.precio_tmp)
      }
    },
}
</script>