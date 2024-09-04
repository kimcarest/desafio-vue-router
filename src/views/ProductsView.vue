<template>
    <Card 
      :data="{
          nombre: nombre,
          descripcion: descripcion,
          precio: precio,
          cantidad: cantidad,
      }"
    />

    <div class="text-center mb-3">
      <router-link 
          class="btn btn-outline-success fs-1"
          to="/"
      >Volver al home</router-link>
  </div>
</template>

<script>

import Card from '../components/Card.vue'

export default {
  components: {
      Card
  },
  props: {
      nombre: {
          type: String,
          required: true
      },
      descripcion: {
          type: String,
          required: true
      },
      precio: {
          type: String,
          required: true
      },
      cantidad: {
          type: String,
          required: true
      },
  }
}
</script>