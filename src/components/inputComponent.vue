<template>
    <ion-input id="id" :value="value" :Type="type" placeholder="placeholder" label="label"></ion-input>
  </template>
  
  <script lang="ts">
  import { IonInput } from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    components: { IonInput },
    props: {
      type: String,
      id: {
        type: String,
        required: true
      },name: String,
      value: String,
      paceholder: String,
      clearInput: Boolean,
      debounce: Number,
      disabled: Boolean,
      maxlength: Number,
      min: Number,
      max: Number,
      step: Number
    }
  });
  </script>
  
  <style scoped>
  /* Estilos del componente */
  /* Estilos globales */
  </style>