<template>
  <div class="about">
    <section class="login">
      <section class="container-fluid bg">
        <section class="row justify-content-center pt-5 pb-5">
          <section class="col col-sm-6 col-md-6 col-lg-4">
            <form class="form-container">
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
                <label for="exampleInputEmail1">correo electronico </label>
                <input
                  type="email"
                  class="form-control"
                  id="exampleInputEmail1"
                  aria-describedby="emailHelp"
                />
              </div>
              <div class="form-group">
                <label for="exampleInputPassword1">Contraseña</label>
                <input
                  type="password"
                  class="form-control"
                  id="exampleInputPassword1"
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
              <button type="submit" class="btn btn-primary btn-block">
                Ingresar
              </button>
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