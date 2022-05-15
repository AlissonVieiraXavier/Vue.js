<template>
 <div class="is-flex is-align-items-center is-justify-content-space-between">
                <CronoMetro :tempoEmSegundos="tempoEmSegundos"/>
                <button class="button" @click="iniciar">
                    <span class="icon">
                        <i class="fas fa-play"></i>
                    </span>
                    <span>play</span>
                </button>
                <button class="button" @click="encerrar">
                    <span class="icon">
                        <i class="fas fa-stop"></i>
                    </span>
                    <span>stop</span>
                </button>

                </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import CronoMetro from './Cronometro.vue'



export default defineComponent({
    name: "TempoRizador",
    data(){
        return{
          tempoEmSegundos:0,
          cronometro:0,
        }
    },
    components: {
      CronoMetro,
    },
    methods:{
        iniciar(){
            this.cronometro = setInterval(()=>{
                   this.tempoEmSegundos += 1;
            },1000)
     
        },
        encerrar(){
          clearInterval(this.cronometro);
        }
    }

})
</script>