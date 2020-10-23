<template>
        <div class="card" style="width: 18rem;">
      <img :src="imagen.img_product" class="card-img-top" alt="...">
      <div class="card-body">
        <p class="card-text">{{imagen.nombre}}</p>
      </div>
    </div>
</template>

<script>
export default {
    name: 'Imagen',
    props: ['imagen']
}
</script>