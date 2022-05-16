<template>
<div class="box has-text-weight-bold tarefa">
<div class="columns">
    <div class="column is-7">
        Descrição da tarefa
    </div>
    <div class="column">
    <CronoMetro tempoEmSegundos="15"/>
</div>
</div>

</div>

</template>
<script lang="ts">

import { defineComponent } from "vue";
import CronoMetro from './Cronometro.vue'
export default defineComponent({
    name:"TarefA",
    components:{
        CronoMetro,
    }

})
</script>
<style scoped>
.box{
    background:linear-gradient(#fdce72,#fdcf72dc,#fdcf7293);
}


</style>

