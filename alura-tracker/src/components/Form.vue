<template>
   <div class="box">
        <div class="columns">
            <div class="column is-8" role="form" aria-label="Formulario para criação de nova tarefa">
                <input 
                type="text" 
                class="input" 
                placeholder="Digite aqui a tarefa que você deseja iniciar"
                >
            </div>
            <div class="column">
               <TempoRizador/>
               

            </div>
       
        </div>
   </div>

</template>
<script lang="ts">
import { defineComponent } from "vue";
import TempoRizador from './Temporizador.vue'

 export default defineComponent({
     name: "FormuLario",
     components: {
        TempoRizador,
        },
 })

</script>

<style>

</style>