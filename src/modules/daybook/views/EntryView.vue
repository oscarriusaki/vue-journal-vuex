<template>
  <div class="entry-title d-flex jsutify-content-between p-2">
    <div>
      <span class="text-success fs-3 fw-bold">15</span>
      <span class="mx-1 fs-3 fw-bold">Julio</span>
      <span class="mx-2 fs-4 fw-light">2021, jueves</span>
    </div>
    <div>
      <button class="btn btn-danger mx-2">
        Borrar
        <i class="fa fa-trash-alt"></i>
      </button>
      <button class="btn btn-primary">
        Subir foto
        <i class="fa fa-upload"></i>
      </button>
    </div>
  </div>
  <hr>
  <div class="d-flex flex-column px-3 h-75">
    <textarea
      placeholder="Que sucedio hoy"
    >

    </textarea>
  </div>
  <FabVue icon="fa-save"/>
  <img 
    src="https://w0.peakpx.com/wallpaper/816/168/HD-wallpaper-sasuke-uchiha-head-black-hair-anime-naruto-shippuuden-naruto.jpg" 
    alt=""
    class="img-thumbnail"
    >
</template>

<script>
import { defineAsyncComponent } from 'vue'
export default {
  components: {
    FabVue: defineAsyncComponent(() => import(/* webpack */ '../components/FabVue.vue'))
  }
}
</script>

<style lang="scss" scope>
textarea{
  font-size: 20px;
  border: none;
  height: 100%;
  &:focus {
    outline: none,
  }
}
img{
  width: 200px;
  position: fixed;
  bottom: 150px;
  right: 20px;
  box-shadow: 0px 5px 10px   rgba($color: #000000, $alpha: 0.2)
}
</style>