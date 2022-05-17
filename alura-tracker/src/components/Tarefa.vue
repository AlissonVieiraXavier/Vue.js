<template>
<div class="box has-text-weight-bold tarefa">
<div class="columns">
    <div class="column is-7">
        {{tarefa.descricao}}
    </div>
    <div class="column">
    <CronoMetro :tempoEmSegundos="tarefa.duracaoEmSegundos"/>
    </div>
</div>

</div>

</template>
<script lang="ts">

import ITarefa from "../interfaces/ITarefa";
import { defineComponent,PropType } from "vue";
import CronoMetro from './Cronometro.vue'
export default defineComponent({
    name:"TarefA",
    components:{
        CronoMetro,
    },
    props:{
        tarefa:{
            type: Object as PropType <ITarefa>,
            required: true,
        }
    },

})
</script>
<style scoped>
.box{
    background:linear-gradient(#fdce72,#fdcf72dc,#fdcf7293);
}


</style>

