<template>
    <Navbaru/>
        <div class="container">
            <nav class="navbar navbar-light navbar-expand-sm" style="background-color: #f4f9fc;">
                <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarTogglerDemo01" aria-controls="navbarTogglerDemo01" aria-expanded="false" aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
                </button>

                <div class="collapse navbar-collapse" id="navbarTogglerDemo01">
                <div class="navbar-nav mx-auto text-center">
                <a class="nav-link active" href="#" tabindex="-1" aria-disabled="true">Pizzas</a>
                <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Bebidas</a>
                <a class="nav-link" href="#" tabindex="-1" aria-disabled="true">Postres</a>
                </div>
                </div>
            </nav>
        </div>
    <section class="lista Pizza">
        <div class="row justify-content-center">
           <div class="col-sm-6 col-md-6">
               
           </div>
        </div>

    </section>
</template>

<script>
import Navbaru from '@/components/Navbaru.vue'
export default {
    components: {
    Navbaru
  }
}
</script>

<style scoped>

</style>