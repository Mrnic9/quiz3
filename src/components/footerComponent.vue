<template>
  <footer>
    <p>{{ footertext }}</p>
  </footer>
  </template>
  
  <script lang="ts">
  import { IonFooter } from '@ionic/vue';
  import { defineComponent } from 'vue';
  
  export default defineComponent({
    components: { IonFooter },

   data(){
    return{
        footertext:'Hecha por Nicolas Nivera Aroca 2024'
    }
   }

  });
  </script>
  
  <style scoped>
    footer{

    background-color: lightcyan;
    position: absolute;
    bottom: 0;
    width: 100%;
    height: 40px;
    color: black;
    align-items: center;
    justify-content: center;

    }
  </style>