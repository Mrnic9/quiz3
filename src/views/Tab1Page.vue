<template>
  <ion-page>
    <ion-header :translucent="true">
      <ion-toolbar>
        <ion-title>Formulario de Ingreso</ion-title>
      </ion-toolbar>
    </ion-header>

    <ion-content :fullscreen="true">
     
      <div id="form">
      
        <div id="description">
          <p>Bienvenido </p>
        </div>
        <div>
          <ion-searchbar placeholder="Consultar "></ion-searchbar>
        </div>
        <div >
          <InputComponent id="User" name="Nombre" label="Nombre: " placeholder="Nombre"/>
          <InputComponent  id="Fecha" Type=date name="password"  label="Fecha: " />
          <InputComponent id="Celular" type=number name="Celular" label="Celular" placeholder="Celular"/>
          <InputComponent id="Correo" type=text name="Correo" label="Correo" placeholder="Correo"/>

        </div>

        <div>
          <buttonComponent id="save" value="Guardar" fill="outline" color="success"/>
          <buttonComponent id="update" value="Modificar" fill="outline" color="warning"/>
          <buttonComponent id="update" value="Eliminar" fill="outline" color="primary"/>
          <buttonComponent id="update" value="Consultar" fill="outline" color="light"/>
        </div>

      </div>
   
    </ion-content>
   <footer>
    <footerComponent/>
   </footer>
  </ion-page>
</template>

<script setup lang="ts">
import { IonPage, IonHeader, IonToolbar, IonTitle, IonContent ,IonCard} from '@ionic/vue';
import buttonComponent from '@/components/buttonComponent.vue';
import InputComponent from '@/components/inputComponent.vue';
import footerComponent from '@/components/footerComponent.vue';

</script>

<style scoped>





</style>
