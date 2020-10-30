<template>
      <div id="nav">
        <router-link to="/inicio">Inicio</router-link> |
        <router-link to="/login">Ingresar</router-link>
    </div>
  <div class="about">
    <section class="login">
      <section class="container-fluid bg">
        <section class="row justify-content-center pt-5 pb-5">
          <section class="col col-sm-6 col-md-6 col-lg-4">
            <form class="form-container" @submit.prevent="login">
              <div class="form-group text-center">
                <label>Iniciar Sesion</label>
              </div>
              <div class="form-group text-center">
                <label
                  >Accede a tus pedidos favoritos, guarda tus direcciones y pide
                  de forma fácil y rápida.</label
                >
              </div>
              <div class="form-group">
                <label for="nombre">Nombre </label>
                <input
                  type="text"
                  class="form-control"
                  id="nombre"
                  aria-describedby="emailHelp"
                  v-model="nombre"
                />
              </div>
              <div class="form-group">
                <label for="password">Contraseña</label>
                <input
                  type="password"
                  class="form-control"
                  id="password"
                  v-model="password"
                />
              </div>
              <div class="form-group">
                <div class="form-group form-check">
                  <input
                    type="checkbox"
                    class="form-check-input"
                    id="exampleCheck1"
                  />
                  <label class="form-check-label" for="exampleCheck1"
                    >Recordar cuenta</label
                  >
                </div>
              </div>
              <button class="btn btn-primary btn-block" type="submit">Ingresar</button>
             
              <div class="form text-center">
                <label class="text-center" for="google">O con </label>
              </div>
              <div class="form-group">
                <button type="submit" class="btn btn-block bt">Google</button>
              </div>

              <div class="form">
                <label for="registra">No tienes cuanta</label>
                <a href="#">Registrar ahora</a>
              </div>
            </form>
          </section>
        </section>
      </section>
    </section>
  </div>
</template>

<script>
// @ is an alias to /src
import axios from 'axios'
export default {
  name: 'Login',
  data(){
    return {
      nombre: "",
      password: "",
      error: false
    }
  },
  methods:{
    //Iniciamos el proceso de consumo del api rest de django
    login(){
      this.error=false
      axios.post("http://127.0.0.1:8000/auth/",{
        username: this.nombre,
        password: this.password
      },{
        headers: {
          'Content-Type':'application/json',
          //"Authorization": "JWT " + localStorage.getItem("token")
        }
      })
      .then((response)=>{
        //console.log(response.data)
        localStorage.setItem('token', response.data.token)
        this.$router.push('/inicio')
      })
    }
  }
}
</script>



<style>
.login {
  background-image: url("../assets/img/fondo2.jpg");
  background-repeat: no-repeat;
  background-size: cover;
}

.form-container {
  background: #f9e7d6;
  padding: 30px;
  border-radius: 10px;
  box-shadow: 0px 0px 10px 0px #000;
}
.bt {
  background: #dd4b39;
  color: white;
}
#nav{
        background:#F7C700;
    }

/* adminstrador */

.menu-section {
  background: #324a5b;
}
.color-principal {
  background: #324a5b;
  color: white;
}
.contenido {
  background: #f1f8f9;
}
.bgnav {
  background: #324a5b;
}
.piza {
  color: white;
}
.adm {
  color: white;
}
.adm:hover {
  color: white;
}

.menu {
  padding-top: 10px;
}
.pagine {
  border: 1px solid black;
}
</style>