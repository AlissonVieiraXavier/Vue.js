<template>
    <main class="columns is-gapless is-multiline">
      <div class="column is-one-quarter">
        <BarraLateral/>
      </div>
      <div class="column is-three-quarter">
       <FormuLario/>
      </div>
      <div class="lista">
        <TarefA/>
        <TarefA/>
        <TarefA/>
        <TarefA/>
      </div>
    </main>
</template>

<script lang="ts">
import { defineComponent } from 'vue';
import BarraLateral from './components/BarraLateral.vue'
import FormuLario from './components/Form.vue'
import TarefA from './components/Tarefa.vue'

export default defineComponent({
  name: 'App',
  components: {
    BarraLateral,
    FormuLario,
    TarefA,
  }
});
</script>

<style>
@media screen and (min-width: 768px){  
  .lista{
    position: relative;
    margin-top: -500px;
    width: 70%;
    left: 27%;
    padding-top:20px;
    }
}

</style>

